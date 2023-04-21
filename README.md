### 참조 자료 링크

> - [OpenJDK](https://www.azul.com/downloads/?version=java-19-sts&os=macos&architecture=arm-64-bit&package=jdk)
> - [node.js](https://nodejs.org/en/)
> - [Docker](https://www.docker.com/)
> - [Mariadb](https://mariadb.org/)
> - [DBeaver](https://dbeaver.io/)
> - [Eclipse](https://www.eclipse.org/)
> - [Apache](https://apache.org/)
> - [Apache Project](https://apache.org/index.html#projects-list)
> - [Http Server](https://httpd.apache.org/)
> - [Homebrew](https://brew.sh/index_ko)

# MAC 사용자가 시작한 프로그램

### 0. Shell Foder

<img src="./images/web.png" width="1920"></img>

### Homebrew 설치

```
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Homebrew 환경설정 보기

```
  /opt/homebrew/bin/brew config
```

#### /usr/local → /opt/homebrew 수정이 필요

### 해결 방안

```
  /opt/homebrew/bin/brew doctor
```

```
  echo 'export PATH="/opt/homebrew/bin:$PATH"' >> ~/.zshrc
```

### brew config 확인

```
  HOMEBREW_PREFIX: /opt/homebrew
```

### Homebrew 버젼 확인

```
  brew -v
```

----
### YouTube Link

> * [Java Install](https://youtu.be/VvQTz_Ux8Tc)
> * [Node.Js Install](https://youtu.be/_lEQlgFijc4)
> * [Docker Install](https://youtu.be/jBVTQf_tJj0)
> * [MariaDB Install](https://youtu.be/QuPLYFJsfk8)
> * [DBeaver Install](https://youtu.be/TeWB8BqrVbQ)
> * [Eclipse Install](https://youtu.be/EnkS9WEf5uM)
> * [Httpd Install](https://youtu.be/EDfejcrF1yo)
> * [Tomcat Install](https://youtu.be/MfM6djlJUhM)

---

# Table of Contents

#### 0. Shell Foder

##### [1. Java](./page/java)

##### [2. NodeJs](./page/node)

##### [3. Docker](./page/docker)

##### [4. MariaDB](./page/mariadb)

##### [5. DBeaver](./page/dbeaver)

##### [6. Eclipse](./page/eclipse)

##### [7. Httpd](./page/httpd)

##### [8. Tomcat](./page/tomcat)
