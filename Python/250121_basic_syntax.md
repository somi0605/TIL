# 문자열
## 적절한 변수명 설정
- student_name = '홍길동'
- student_age = 20
- label_student_name = '이름 : ' #label 해당 변수가 출력될 데이터의 제목
- label_student_age = '나이 : '
- message_intro = '학생 정보를 출력합니다.' #출력될 메세지의 목적이나 역할을 설명명
- message_details = '각각의 정보는 다음과 같습니다'
- message_complete = '출력 완료'

>[!IMPORTANT]
>PEP-8은 파이썬 코드 작성 시 가독성과 일관성을 높이기 위해 제안된 스타일 가이드(협업 시 코드의 품질과 이해도를 높이는 데 매우 중요)

## TYPE 설정하기
```bash
print(type(string))
print(type(integer))
print(type(floating_point))
print(type(a_list))
print(type(dictionary))
print(type(a_set())
print(type(a_range))
print(type(a_tuple))
print(type(boolean))
```

```bash
print(f'{twinkle} {little} {star} {beautiful}\n {east_sky}{eseodo} {west_sky}{eseodo}\n {twinkle} {little} {star} {beautiful}')
```

>[!NOTE]
>\n 은 엔터 cf) window http에서는 \r\n
 ## 슬라이싱
- f-string에 little_star[0:2] 자체를 넣어도 된다
- little_star[0:2] 대신 little_star[:2]로 더 간결하게

- a = password[66:69]
```bash
third_word = a[::-1] #문자열 역순
``` 
## float 실수형 
### 부동소수점 
- 원주율 3.1415926535897932384626433832795028841971693993751058209749445923078164062862089986280348253421170679
- 반지름 15

pi = 3.1415926535897932384626433832795028841971693993751058209749445923078164062862089986280348253421170679
radius = 15

label_pi = '원주율 : '
label_radius = '반지름 : '
label_circumference = '원의 둘레 : '
label_area = '원의 넓이 : '

```bash
print(f'{label_pi}{str(pi[:18])}')
# 실패원인) pi(숫자)를 문자열로 변환하지 않고 인덱싱 함: 부동소수점(float)은 숫자형 데이터 타입이므로 문자열이나 리스트처럼 인덱싱([])이 불가능
```

### 방법1 round 사용
```bash
pi = round(pi, 15) #재할당: 위의pi는 저대로 끝
print(f'{label_pi}{pi}')
print(f'{label_radius} {radius}')
print(f'{label_circumference} {radius*2*pi}') #f-string은 중괄호 {} 안에 파이썬 표현식을 넣어야 제대로 동작
print(f'{label_area}{radius*radius*pi}')
```

### 방법2 f-string 소수점 사용
```bash
print(f'{pi:.15f}')
```
### 방법3 그냥 print 해도 제한이 걸려서 주어진 소수점까지만 나옴
```bash 
print(pi)
```
>[!IMPORTANT] 
>pwd: print working directory 현재 작업 디렉토리(현재 위치)를 확인하는 명령어

