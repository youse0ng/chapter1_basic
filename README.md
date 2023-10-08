![스크린샷 2023-10-08 170000](https://github.com/youse0ng/chapter1_basic/assets/130890430/4720e4ac-e324-4329-a712-da21bf2003bc)

깃과 깃허브 첫 실습

1. git init 명령어
Initalized empty Git repository in {프로젝트 경로}/.git 이런 문구가 뜬다면 .git 폴더가 생성됐으니 이 프로젝트는 깃으로 소스코드 버전관리가 되겠구나

2. git config 명령어: 깃 지역 저장소에 사용자 등록

md=MarkDown 형식의 파일을 의미하는데, 
README.md 파일을 생성하면 해당 원격 저장소의 메인 페이지로 작동한다.
이러한 이유로 프로젝트에 대한 설명, 설치방법 등을 설명하는데 README.md를 사용한다.

3. git add 명령어: 
git add README.md 파일을 커밋에 포함될 파일로 등록한다.

4. git commit -m '저장소 설명 추가': 새로운 커밋 생성
-m 옵션은 생성하는 커밋의 메세지를 작성하는 기능을 제공

5. git log 명령어: 커밋이 잘 생성되었는지 확인

---

여기까지 지역 저장소에 새로운 커밋 생성을 완료했다 이제 생성된 커밋을 원격 저장소에 등록해보자.

1. youse0ng/chapter1-basic 레포지토리(원격 저장소)를 생성하고

2. 원격 저장소의 주소를 복사해서 지역 저장소에 알려줄 필요가 있다. 목적은 지역 저장소의 커밋을 원격 저장소에 등록하기 위함이다.
https://github.com/youse0ng/chapter1_basic.git

git remote add origin https://github.com/youse0ng/chapter1_basic.git 을 터미널에 실행한다.

3. git push origin main 명령어 :
지역 저장소에서 생성한 커밋을 원격 저장소에 등록

4. 원격 저장소 페이지 접속해서 커밋이 성공적으로 등록되었는지 확인
README.md 파일은 원격 저장소의 메인 페이지 역할을한다. 
README.md 파일의 내용이 메인 페이지에 노출되면 제대로 커밋을 등록한거다.

정리하자면,

깃과 깃허브를 이용해서 지역 저장소에서 커밋을 생성한 후 원격 저장소에 커밋을 등록하는 실습했다.

