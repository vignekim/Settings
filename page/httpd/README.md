### 참조 자료 링크
> * [Apache](https://apache.org/)
> * [Apache Project](https://apache.org/index.html#projects-list)
> * [Http Server](https://httpd.apache.org/)
> * [Homebrew](https://brew.sh/index_ko)

# HTTP (Hypertext Transfer Protocol Daemon)
### 7. Httpd
<img src="../../images/httpd/httpd.png" width="1920"></img>

###### Apache Project List (Http Server -> httpd)
<img src="../../images/apache.png" width="1920"></img>

###### Http Server 선택 시 정보 화면으로 이동
<img src="../../images/httpd/httpd-1.png" width="1920"></img>

###### Homebrew를 이용하여 Httpd 설치
```
    brew install httpd
```

###### Homebrew를 이용하여 Httpd 실행
```
    brew services start httpd
```

###### Homebrew를 이용하여 Httpd 정지
```
    brew services stop httpd
```

###### Homebrew를 이용하여 Httpd 다시 실행
```
    brew services restart httpd
```

----
### docker를 사용하여 설치 할 경우
```
    * 주의 사항 *
    > 기존 서비스 중인 웹서버(httpd)가 있을 경우는 Service를 중단 후 사용 하세요.
    > volumes 설정에 있는 경로가 필수로 있어야 합니다.
      - /Users/계정/www << MAC OS 경우 
```
###### docker-compose.yml 파일 내용
```
    version: "3.7"

    services:
      httpd:
          image: httpd:latest
          ports:
            - 80:80
          volumes:
            - /Users/bean/www:/usr/local/apache2/htdocs
          networks:
            - backend
          restart: always
    networks:
      backend:
```

###### docker-compose.yml 실행 명령어
```
    docker-compose up -d
```

###### docker-compose.yml 정지 명령어
```
    docker-compose down
```

----

# Table of Contents
##### [0. Shell Foder](../../../../)
##### [1. Java](../java)
##### [2. NodeJs](../node)
##### [3. Docker](../docker)
##### [4. MariaDB](../mariadb)
##### [5. DBeaver](../dbeaver)
##### [6. Eclipse](../eclipse)
#### 7. Httpd
##### [8. Tomcat](../tomcat)
