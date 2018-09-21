# Linux

## 용어사전
* RHEL : Red Hat Enterprise Linux

## 툴
- tmux : 여러 tty 전환 가능하게 해주는 프로그램
  - tmux new -s {{console name}} : open new terminal
  - tmux 에서 exit : 터미널 종료
  **일회용 사용은 가능한데, 제대로 사용하는거 연구 필요**

## 기본 커맨드

* ping 8.8.8.8 : 서버에 요청하고 반응시간 확인하기
* curl : 뭐 이것저것 프로토콜 다 됨
- -X GET/POST/PUT {{url}} : 특정 REST 동작 요청
- curl -O https://naver.com/download/hello.zip
- [wget](https://m.blog.naver.com/PostView.nhn?blogId=alkydes&logNo=220593597738&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F) : 설치한다
* touch : 파일 새로 생성, 시간 업데이트 등

  * touch <<filename>> : 생성
  
  * touch -c <<filename>> : 시간 현재로 업데이트
  
* pwd : 파일 디렉토리
* ls : 현재 디렉토리 출력
* nmcli -d : 이더넷 커넥션 테스트
* lscpu : 컴퓨터 성능 확인
* lshw : 하드웨어 정보
* 네트워크 연결 : 
네트워크 컨피겨 파일 - /etc/sysconfig/network-scripts/
네트워크 인터페이스 온 : ifup
* top : 프로세스 리스트 및 하드웨어 리소스 정보
top -u {{username}}
top -O 



## CentOS 핵(버전7)
* 화면크기 조정
- vim /etc/default/grub
- GRUB_CMDLINE_LINUX에 vga=792 추가
- grub2-mkconfig -o /boot/grub2/grub.cfg
- shutdown -r now

## Types

### Red Hat

* Fedora, CentOS, Oracle Enterprise



#### Commands

* [Build a rpm package](https://www.thegeekstuff.com/2015/02/rpm-build-package-example/) : `yum install rpm-build`
* [Custom repo](https://www.digitalocean.com/community/tutorials/how-to-set-up-and-use-yum-repositories-on-a-centos-6-vps) : /etc/yum.repos.d 에 {{name}}.repo 파일 생성
```
[examplerepo]
name=Example Repository
baseurl=http://mirror.cisp.com/CentOS/6/os/i386
enabled=1
gpgcheck=1
gpgkey=http://mirror.cisp.com/CentOS/6/os/i386/RPM-GPG-KEY-CentOS-6
```
* rpm파일 로컬 설치 : rpm -ivh package.rpm, (다른경로 설치) rpm -ivh -r /new/path package.rpm
