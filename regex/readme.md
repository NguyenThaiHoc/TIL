
`
/^/
`
Bắt đầu dòng

`
/$/
`
Kết thúc dòng

`
/\n/
`
Xuống dòng

`
/\d/
`
Số

`
/\D/
`
Ký tự không phải là số

`
/\w/
`
Ký tự số và chữ

`
/\W/
`
Ký tự không phải là số và chữ

`
/\s/
`
Ký tự dấu cách

`
/\S/
`
Ký tự không phải là dấu cách

`
/\t/
`
Tab

`
/\r/
`
Xuống dòng


`
/\v/
`
Tab dọc

`
/\b/
`
Ký tự không phải là chữ và số bao chữ và Số

`
/\B/
`
là ký tự chữ số bao khối ký tự là chữ số

`
/\bx\b/
`
Ký tự không phải là chữ và số, ký tự x, ký tự không phải là số và chữ

`
/(?:)/
`
Có chứa nhưng không bắt chuỗi sau ?:

`
/(?!)/
`
Không được là ký tự sau ?!
//
`
/(?=)/
`
Phải là ký tự sau ?=

`
/[a-z]/
`
Một ký tự trong khoảng từ a đến z

`
/x+/
`
Một hoặc nhiều ký tự x

`
/x*/
`
Không ,một hoặc nhiều ký tự x


`
/a.*?x/
`
Ký tự a, các ký tự không chứa x, ký tự x (a, và khoảng ngắn nhất đến x)


`
/a[^x]/
`
Ký tự a và một ký tự khác ký tự x

`
/([a-c])x([a-c])x\1x/
`
Một ký tự từ a đến c, một ký tự x, một ký tự từ a đến c, một ký tự x, một ký tự giống trong ngoặc đơn thứ nhất, một ký tự x


`
/a{1,5}/
`
Một đến năm ký tự a

`
/a{2,}/
`
Hơn hai ký tự a

`
/a{2}/
`
Hai ký tự a


`
[a|x]
`
Ký tự a hoặc ký tự x

###### Ví dụ

`
/^\n+/
`
Bắt đầu dòng, nhiều ký tự xuống dòng

`
/^( {4}[^\n]+\n*)+/
`
Bắt đầu dòng, 4 dấu cách,  nhiều hơn 1 ký tự khác xuống dòng, nhiều ký tự xuống dòng,  nhiều hơn 1 khối tương tự


`
/^( *[-*_]){3,} *(?:\n+|$)/
`
Bắt đầu dòng, có thể có 1 hoặc nhiều dấu cách, nhiều hơn 3 của tổ hợp các dấu (-*_),  có thể có một hoặc nhiều dấu cách, xuống dòng hoặc kết thúc dòng và không bắt chuỗi này

`
/^( *>[^\n]+(\n(?!def)[^\n]+)*\n*)+/
`
Bắt đầu dòng, không, một hoặc nhiều ký tự cách,  ký tự >, một hoặc nhiều ký tự khác xuống dòng, xuống dòng nhưng không bắt đầu bằng 'def', một hoặc nhiều ký tự khác xuống dòng, không, một hoặc nhiều ký tự xuống dòng, nhiều khối như vậy


`
/abc(?=d)/
`
Bắt đầu là abc nhưng sau đó phải là d
