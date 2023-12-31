# Python 기초 문법 정리 for 코딩테스트

- `[::-1]` : 문자열 거꾸로 출력
- `print(*)` : 한 칸씩 띄우고(공백) 출력
- `set()` : 중복되지 않은 값을 순서없이 보관하는 자료구조
- `eval()` : 문자열로 표현되는 표현식을 실행해서 결괏값을 받아오는 함수
  ```python
  exp = "1 + 2"
  result = eval(exp)
  print(result) # 3
  ```

- sort : 원본 자체 정렬
- sorted : 새로운 list 반환
- lambda : 익명 함수를 지칭하는 용어
  ```python
  # 1. 첫 번째 인자를 기준으로 오름차순 정렬
  # 2. 두 번째 인자를 기준으로 내림차순 정렬
  arr.sort(key = lambda x : (x[0], -x[1]))
  ```
- `sum()` : 배열의 요소 합
- `Counter(arr).most_common()` : [(-2, 2), (-1, 2), (-3, 1)]
  - (왼쪽 : 값, 오른쪽 : 요소 개수) && 오름차순 정렬함
  - `from collections import Counter`
- `max()` & `min()` : 요소 중 최댓값 & 최솟값
- `len(str(M))` : M이 정수일 때, 자릿수를 구하는 방법
- `ord(문자)` : 유니코드 정수 출력
- `chr(정수)` : 유니코드 문자 출력
- `str[4:-4]` : 문자열 자르기 - 앞에서 5번째 문자열부터 뒤에서 5번째 문자열까지 자르기
- `deque.popleft()` = `list.pop(0)`
- `rstrip()` : 오른쪽 공백 제거 (보통 string을 입력값으로 적을 때, 자주 씀)
- `input()[1:-1].split(',')` : [1, 2, 3, 4] => 1 2 3 4

```python
string = "abcd"

d = string[1:2] # b
s = string[:2] # ab
t = string[2:] # cd
a = string[-1] # d
b = string[-2] # c
c = string[-2:] # cd
k = string[-2:4] # cd

lst = ['a', 'b', 'c', 'd']
s = ''.join(lst) # abcd
s = ', '.join(lst) # a, b, c, d
```
