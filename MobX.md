## mobx에서 functional component를 쓰려면?

`mobx에서 functional component를 쓰기위해 지원해야할 훅이
mobx-react v6부터인데
그렇게되면 mobx의 버전을 올려야한다.
mobx V5로.
그런데 mobx v5는 ie 11이하를 지원하지 않는 문제가 있다.`

대응 방법은,
1. store에 직접적으로 접근하는 page container 단위의 component들은 class component로 가고 props를 통해서만 작동 재사용되는 컴포넌트들은 funtional로 가는 것
2. 전부다 그냥 class 형태로 가는 것
