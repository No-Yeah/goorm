# goorm

[지송함미다. 개발은 쥐약이애오]

- 실행 방법
  1. docker pull ghcr.io/no-yeah/groom/groom_noyeah_spring:0.1 // 퍼블릭 이미지 다운로드
  2. docker-compose.yaml 예시 파일 다운로드 후 수정
     // default로 volume을 /tmp에 마운트되게 해놓았습니다. 변경이 필요하다면 수정해서 사용하세요.
  4. compose 얌 파일 실행  // docker 버전에 따라서 내부 Version: '3.9'는 커스텀하여 사용하세요.
  docker-compose -f /파일절대경로/spring_noyeah.yaml up -d

- 실행 화면
  1. IP:8080 브라우저 접근
     
  ![image](https://github.com/No-Yeah/goorm/assets/36402738/a79d276c-3d6a-434d-8e2e-add45a7d54cd)

  2. join 기능
     
  ![image](https://github.com/No-Yeah/goorm/assets/36402738/78004587-cb60-420a-99a3-09f4362399c4)

  3. list 기능
     
  ![image](https://github.com/No-Yeah/goorm/assets/36402738/6a3f85de-e8b9-49f7-ba3f-b79321515ea8)

- 개발 환경
Rocky Linux 8 - IntelliJ 2023.x / JDK 11 / Spring WEB

- 이미지 pull 실행 환경
  
doc@docker-M# docker version

Client:
 Version:           20.10.21
 
 API version:       1.41
 
 Go version:        go1.18.1
 
 Git commit:        20.10.21-0ubuntu1~22.04.2
 
 Built:             Thu Mar  2 18:26:04 2023
 
 OS/Arch:           linux/amd64
 
 Context:           default
 
 Experimental:      true

 

Server:

 Engine:
 
  Version:          20.10.21
  
  API version:      1.41 (minimum version 1.12)
  
  Go version:       go1.18.1
  
  Git commit:       20.10.21-0ubuntu1~22.04.2
  
  Built:            Wed Feb 15 15:26:57 2023
  
  OS/Arch:          linux/amd64
  
  Experimental:     false
  
 containerd:
  Version:          1.6.12-0ubuntu1~22.04.1
  
  GitCommit:        
  
 runc:
 
  Version:          1.1.4-0ubuntu1~22.04.1
  
  GitCommit:        
  
 docker-init:
 
  Version:          0.19.0
  
  GitCommit:        
  




doc@docker-M# docker-compose version

docker-compose version 1.29.2, build unknown

docker-py version: 5.0.3

CPython version: 3.10.4

OpenSSL version: OpenSSL 3.0.2 15 Mar 2022





doc@docker-M# cat /etc/issue

Ubuntu 22.04 LTS \n \l




doc@docker-M# uname -a

Linux docker-M 5.15.0-25-generic #25-Ubuntu SMP Wed Mar 30 15:54:22 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux


