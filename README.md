## 사전 준비

1. git(git bash) 설치

2. github에 20223578.github.io 저장소 생성 

3. ruby, jekyll 설치

## 로컬, 리모트 저장소 연결

1. 20223578.github.io 저장소에서 클론

2. C 밑에 blog 디렉토리 생성

3. git bash에서 blog 디렉토리로 이동

4. blog 디렉토리에서 git clone <클론한거 붙여넣기>

5. blog 밑에 20223578.github.io 디렉토리 생성완료

## 블로그 생성

1. git bash에서 20223578.github.io 디렉토리로 이동

2. jekyll new . --force

3. bundle add webrick

4. git add, commit, push

5. github에서 블로그 생성 확인

## 테마 적용

1. gitbook 홈페이지에서 클론

2. blog 디렉토리에서 git clone <클론한거 붙여넣기>

3. 새로 생긴 lanyon 디렉토리의 내용물 전부 20223578.github.io 디렉토리에 덮어씌움

5. _config.yml에서 title을 20223578 My blog로 수정

6. _config.yml에서 url과 baseurl을 'https://20223578.github.io/'로 수정

7. git add, commit, push

8. github 블로그에서 테마 적용 확인

## 댓글 기능 구현

1. disqus 회원가입

2. 플랫폼은 jekyll 선택

3. website url은 내 블로그 주소로 설정

4.  _config.yml 파일에 disqus 설정 추가

5. disqus 홈페이지에서 Universal Code 복사

6. 복사해온 코드를 _layouts/post.html에 붙여넣기

7. 주석 해제 후 PAGE_URL, PAGE_IDENTIFIER 설정

8. s.src 내 주소로 되있는거 확인

9. 댓글 기능을 구현할 post파일(임시로 만든 example 파일)에 comments: True 추가

10. MongoDB 정리 포스트에 댓글 기능 구현 확인(구현 되는데 조금 오래걸림)