## auto-closing-tag-in-textarea

웹사이트에서도 코드 편집기처럼 자동으로 태그를 닫아주는 함수를 지원하는 라이브러리입니다.

use :

```
yarn add auto-closing-tag-in-textarea
```

```jsx
import autoClosingTag from 'auto-closing-tag-in-textarea'
import React, { useState } from 'react'

const App = () => {
	const [contents, setContents] = useState('')

	return (
		<div>
			<input type="text" onChange={(e) => setContents(autoClosingTag(e))} value={contents} />
		</div>
	)
}
```
