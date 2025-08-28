React
[lazy](https://react.dev/reference/react/lazy)
[suspense](https://react.dev/reference/react/Suspense)
[animal info](https://github.com/miloupark/Animal-info/pull/7)

## lazy

컴포넌트를 바로 불러오지 않고, 실제로 그 컴포넌트가 필요할 때 불러옴

import Main from "./Main.jsx"
const Main = lazy(()=> import("./Main.jsx"))

## suspense

컴포넌트를 불러오는 동안 사용자에게 보여줄 임시 화면 설정
<Suspense fallback ={"로딩중..."}><Main /></Suspense>
메인이 로딩되는 동안 fallback을 보여주게 된다.
