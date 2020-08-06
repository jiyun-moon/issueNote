# Javascript Thousand Separator
천단위로 콤마 찍어주기.


const format = num =>
    String(num).replace(/(?<!\..*)(\d)(?=(?:\d{3})+(?:\.|$))/g, '$1,');

format(123456789);

결과: 123,456,789
