>1. EC2 운영
>	물리적인 작업은 클라우드 환경이 아니라면 현지에 가서 직접 케이블을 연결하여 작업하는 경우가 많다. 
>	EC2는 관리 콘솔에서 작업할 수 있다. 
>	소프트웨어적인 작업은 클라우드가 아닌 환경이든 EC2이든 관계없이 ssh를 이용해 원격으로 로그인하여 작업한다. 따라서  EC2도 ssh로 접속하도록 설정하는 것은 동일한다. 

>2. EC2 서비스의 기능
>	EC2 서비스에는 인스턴스, AMI, 키 페어 등의 기능 
>	
>	-인스턴스: Aws 클라우드에 생성한 가상 서버를 의미한다. AMI로 몇번이고 같은 구성의 서버를 생성할 수 있기 때문에 생성한 서버를 이와 같이 부른다. 
>	
>	-AMI: 가상 이미지. 인스턴스를 생성하는 기준이 되는 금형과 같은 것이다. OS만 설치된 간단한 유형부터 소프트웨어도 설정된 유형까지 다양한 AMI가 있다. 
>	
>	-키 페어: 인스턴스에 접속할 때 인증을 위해 사용하는 키이다. 
>	
>	-EBS: AWS 클라우드에서 사용할 수 있는 스토리지이다. 
>	
>	-보안 그룹: 가상 방화벽으로, 1개 이상의 인스턴스 트래픽을 제한한다. 
>	
>	-Elastic IP 정적(고정) IPv4 주소이다. 

>3. EC2의 사용 절차
>	1. AWS에 로그인한다.
>		1. 리전을 선택하고 관리 콘솔을 연다
>		2. EC2 대시보드를 연다.
>	2. EC2 인스턴스를 생성한다. 
>		1. AMI를 선택한다.
>		2. 인스턴스 유형을 선택한다. 
>		3. 네트워크와 IP주소를 할당한다. 
>		4. 스토리지를 추가한다.
>		5. 보안 그룹을 설정한다. 
>		6. 키 페어를 선택한다. 
>	3. EC2에 접속한다. 
>		1. ssh로 EC2에 접속한다. 
>	4. 소프트웨어를 설치하고 설정한다. 
>		1. 소프트웨어 설치
>		2. 소프트웨어 설정

>4. 인스턴스 설정 항목
>	일반적인 서버를 생성할 때 검토해야 할 내용은 인스턴스 생성때도 마찬가지이다. 예를 들면 CPU xx, 메모리는 OO, OS는 xx, 웹 서버는 아파치를 설치한다. 하지만 AWS의 경우는 다양한 인스턴스 유형과 여러 AMI를 제공하고 있어 적당히 고르면 된다. 


