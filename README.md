# bbSelenium

## 💽설치 안내(Installation Process)
```bash
git clone https://github.com/juyeori/bbSelenium.git
```

## 📱프로젝트 사용법 (Getting Started)
1. 코드 중 아래 부분에서 자신의 크롬 드라이버 경로 입력
```python
#url 및 웹드라이버 설정
URL = 'https://eclass2.ajou.ac.kr/webapps/discussionboard/do/message?action=list_messages&course_id=_52212_1&nav=discussion_board&conf_id=_58228_1&forum_id=_57761_1&message_id=_'
driver = webdriver.Chrome(executable_path='드라이버 주소') #, options = webdriver_options)
driver.get(url = URL)
```

2. 코드 중 아래 부분에서 black board 아이디와 비밀번호를 입력
```python
# 로그인
driver.find_element_by_id('userId').send_keys('아이디')
driver.find_element_by_id('password').send_keys('비밀번호')
```

3. 코드 중 아래 부분에서 정리된 내용을 추출할 경로 입력
```python
#데이터 프레임 변환 후 csv로 추출
df = pd.DataFrame(story, name)
speaker = input()
df.to_csv("파일경로/%s" %(speaker), encoding="utf-8-sig")
```

3. ctrl + Enter
4. 추가적인 입력 칸이 뜨면, 그 칸에 추출한 내용을 엑셀 파일로 저장하기 위한 파일명 입력
