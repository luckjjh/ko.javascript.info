importance: 4

---

# 정렬 기능을 제공하는 표

열 제목을 나타내는 요소인 `<th>`를 클릭하면 열 전체가 정렬되는 표를 만들어보세요.

모든 `<th>` 속성엔 다음과 같이 데이터의 타입이 정의되어 있습니다.

```html
<table id="grid">
  <thead>
    <tr>
*!*
      <th data-type="number">나이</th>
      <th data-type="string">이름</th>
*/!*
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>5</td>
      <td>일리야</td>
    </tr>
    <tr>
      <td>10</td>
      <td>보라</td>
    </tr>
    ...
  </tbody>
</table>
```

위 예시에선 첫 번째 열엔 숫자가, 두 번째 열엔 문자열이 들어갑니다. 구현할 정렬 함수는 데이터 타입에 맞게 정렬을 해줘야 합니다.

이 문제에선 `'숫자'`와 `'문자열'` 타입만 다룬다고 가정하겠습니다.

제대로 해답을 작성했다면 다음 예시처럼 동작해야 합니다.

[iframe border=1 src="solution" height=190]

P.S. The table can be big, with any number of rows and columns.
