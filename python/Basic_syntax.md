## 표현식과 값
### 표현식
- 값으로 평가할 수 있는 코드 조각

### 값 
- 표현식이 평가된 결과
- 평가 : 표현식을 실행하여 값을 얻는 과정
- 문장 : 실행 가능한 동작을 기술하는 코드
  
## Data Type
1. 값 (피연산자)
- Numeric Type: int, float, complex
- Sequence Type: list, tuple, range
- Text Sequence Type: str
- Non-Sequence Type: set, dict
- 기타: Boolean, None, Function
2. 연산자
- 산술 연산자
- 연산자 우선순위 : ** -> - -> * / // % -> + -

### Numeric Type
1. int
   - 진수 표현
    ```python
    print(0b10) # 2진수
    print(0o30) # 8진수
    print(0x10) # 16진수
    ```
2. float
   - 지수 표현 방식
  ```python
  number = 314e-2
  print(number)
  ```
     - 부동소수점 에러 
       - decimal 모듈을 활용해 정확성 보장 가능
### Sequence Type
**특징**
- 순서: 값들이 순서대로 저장
- 인덱싱: 각 값에 고유한 번호를 가지고 있음, 특정 위치의 값을 선택하거나 수정 가능
- 슬라이싱: 부분적인 값을 추출 가능
- 길이: len()를 통해 저장된 값의 개수를 구할 수 있음
- 반복: 저장된 값들을 반복적으로 처리할 수 있음

1. str
   - 문자들의 순서가 있는 *변경 불가능한* 시퀀스 자료형
   - Escape sequence
     - \사용하여 탈출 가능
   - String Interpolation
     - f-string