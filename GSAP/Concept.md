### Concept

`GSAP`은 웹에서 사용하는 `AfterEffect`와 비슷하다고 생각하다.
타임라인과 Ease와 관련된 다양한 속성 등을 제공해 디테일한 animation의 구현이 가능하다.

```ts
import gsap from 'gsap';

gsap.메서드(ref, { Animation });
```

```tsx
import gsap from "gsap";
import {useRef} from "react"

const button = () => {
	const boxRef = useRef(null);

	const clickHandler = () => {
		gsap.from(boxRef.current, {
			autoAlpha: 0, duration: 2
		}
	};

	return (
		<>
			<div ref={boxRef}>Box</div>
			<button onClick={clickHandler}></button>
		</>
	);
}
```
