# 모바일 사파리 fixed bug
## 모바일 사파리 브라우저에서 전체 길이에 영향을 주는 클릭이 일어난 경우 최 상단에 의문의 라인이 생기면서 헤더 위에 미세한 영역이 노출되는 현상

html,body{
    -webkit-overflow-scrolling : touch !important;
    overflow: auto !important;
    height: 100% !important;
}


* 참조1: https://www.eventbrite.com/engineering/mobile-safari-why/
* 참조2: https://stackoverflow.com/questions/29001977/safari-in-ios8-is-scrolling-screen-when-fixed-elements-get-focus
