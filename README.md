# Docker 설치 및 컨테이너 실행

[Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/8ffb134c-287e-4abc-8c77-edbb340b0463/22facaae-3adc-4e62-bf27-d55ec7aeb201/Untitled.pdf)

1. Docker 를 컴퓨터에 설치하고 이미지 띄워보기
2. Docker 공식 사이트([링크](https://www.docker.com/get-started/))에 접속해 Docker Desktop 설치하기
3. Docker 컨테이너 실행하기 : 공식사이트 [링크](https://docs.docker.com/guides/walkthroughs/run-a-container/) 를 참고해 컨테이너를 빌드한 후 실행시켜보세요.

---

**☑️ 1 . 디렉터리에 Git으로 복제하기**

```jsx
git clone https://github.com/docker/welcome-to-docker
```

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/8ffb134c-287e-4abc-8c77-edbb340b0463/6eefff21-875b-41f6-8b83-ffa8e19a1b06/Untitled.png)

**☑️ 2.** 디렉터리 변경 

```jsx
cd /path/to/welcome-to-docker/
```

**☑️ 3.** docker build하기 

```jsx
 docker build -t welcome-to-docker .
```

이전 명령에서 플래그 는 이 경우 `-t`이미지에 이름 태그를 지정했고 . `welcome-to-docker`그리고 `.`Docker는 Dockerfile을 찾을 수 있는 위치를 알 수 있다.

**☑️ 4.**컨테이너 실행 

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/8ffb134c-287e-4abc-8c77-edbb340b0463/68b154cc-1bab-422e-84d8-2dd463bccd5f/Untitled.png)

- docker Desktop 에서 images 선택
- Actions 실행버튼을 누른다

**☑️ 5.**호스트 Port번호 입력 후 Run실행 

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/8ffb134c-287e-4abc-8c77-edbb340b0463/4177a447-7e3b-427b-871b-d9c942aa77f8/Untitled.png)

**☑️ 6.**http://localhost:8089/ 로 접속 테스트 

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/8ffb134c-287e-4abc-8c77-edbb340b0463/d509f5f9-447a-4d48-80d0-4b9d9d3803f1/Untitled.png)

이렇게 성공화면이 뜨는걸 확인할 수 있다

- welcome-docker 컨테이너를 8089:3000 포트로 실행중 일 때
호스트의 8089포트로 접속하면, welcome-docker 컨테이너로 연결이된다고 이해하면 된다.
- Docker는
