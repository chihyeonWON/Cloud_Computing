# Cloud_Computing
컴퓨터공학과 클라우드컴퓨팅 정리입니다.
```
하드웨어를 사서 쓰는 게 아니라 임대해서 쓴 만큼 비용을 내는 유틸리티(클라우드) 컴퓨팅

aws를 사용해서 프런트엔드 앱의 백엔드를 구현할 수 있을 

```
![image](https://user-images.githubusercontent.com/58906858/222406453-66464324-ff97-4c87-af19-395645ea4ef5.png)         
![image](https://user-images.githubusercontent.com/58906858/222408060-2f926ee9-583d-4473-a8ee-3861cdd98b5f.png)      
![image](https://user-images.githubusercontent.com/58906858/222409589-9c067e68-727c-4121-bea3-232097596fcc.png)      
![image](https://user-images.githubusercontent.com/58906858/222410544-a778da11-1ef2-42da-8b2e-8755971212a3.png)   
![image](https://user-images.githubusercontent.com/58906858/222413885-af3ddd39-160a-432c-a17b-ab7a0956c19f.png)   
![image](https://user-images.githubusercontent.com/58906858/222414362-c5c8cb0f-4842-4962-883c-2613b066b965.png)
![image](https://user-images.githubusercontent.com/58906858/222414705-5329bd5d-8547-4778-9da4-19e4a5ba42fe.png)   
![image](https://user-images.githubusercontent.com/58906858/222415003-66ca4e86-72f9-480b-b444-7b5bcd42161f.png)   
![image](https://user-images.githubusercontent.com/58906858/222415544-7ded165f-7f6b-4c71-8dd8-fbee96f4dfb6.png)
![image](https://user-images.githubusercontent.com/58906858/222416305-0989dd8a-db99-41de-b7b5-10bd119fba39.png)
![image](https://user-images.githubusercontent.com/58906858/222416329-6c6d5931-8202-4c54-8430-77a2764dbac4.png)

## 클라우드 컴퓨팅의 이해

2023-03-11
```
클라우드 컴퓨팅이란 언제 어디서나 필요한 만큼의 컴퓨팅 리소스를 필요한 시간만큼 인터넷을 통하여 활용할 수 있는 컴퓨팅
방식을 일컫는다.

클라우드 컴퓨팅은 IT 리소스의 유휴 리소스를 활용, 비용 절감 그리고 사용자 맞춤형 서비스 지원을 목적으로 사용되기 시작하였다.
```

## 클라우드 컴퓨팅의 정의

2023-03-13
```
클라우드 컴퓨팅에 대한 정의는 NIST (National Institute of Standards and Technology)에서 제시되었다.
NIST에서는 클라우드 컴퓨팅은 컴퓨팅 리소스(서버, 저장 장치, 애플리케이션, 네트워크 등)에 언제 어디서나 필요에 따라
편리하게 네트워크를 통해 접근하는 기능을 제공하는 모델이다. 컴퓨팅 리소스는 최소한의 관리로 신속하게 프로비저닝되고
배포될 수 있다. (프로비저닝 : IT 리소스를 실시간으로 사용 가능한 상태로 만드는 또는 규격품 형태로 패키징하는 기술을 뜻함)
```

## 클라우드 모델의 5가지 기본 특성
```
On-demad self-service ; 주문형 셀프서비스, 즉 필요한 자원을 사용자가 선택할 수 있다.
Brand Network acess : 광대역 네트워크 접근, 즉 빠른 네트워크 통신망이 필요하다.
Resource Pooling : 리소스 풀링, 다양한 IT 리소스들이 한데 모여 Pool을 이룬다. 즉 모여있어야 한다.
Lapid Elasticity : 빠른 탄력성, 변화하는 환경에 적응이 빨라야 한다.
Measured Service : 서비스는 측정이 가능해야 한다.
```

## 클라우드 모델의 3가지 서비스 모델
```
클라우드 서비스는 제공 범위에 따라서 IaaS, PaaS, SaaS로 구분된다.

IaaS : (Infrastructure as a Service) : CPU, 메모리 등의 H/W 리소스를 제공하는 클라우드 서비스
PaaS : (Platform as a Service) : OS와 S/W 개발이나 데이터 분석을 위한 도구들까지 제공하는 서비스
SaaS : (Software as a Service) : H/W와 OS 뿐만 아니라 응용 S/W(애플리케이션)까지 제공하는 서비스
```

## 클라우드 모델의 4가지 배포 모델
```
1. 퍼블릭 클라우드 (Public Cloud) : 다수의 사용자가 클라우드 제공자가 공급하는 서버 및 저장소와 같은 IT리소스를
공유하여 사용하는 모델을 말한다. 대표적으로 마이크로소프트 Azure, AWS, Google Cloud Platform, Naver Cloud 등이 이 모델에 포함된다.

2. 프라이빗 클라우드 (Private Cloud) : 단일 조직이 독점적으로 데이터 센터를 구축하고 독점적으로 사용하는 컴퓨팅 환경을 의한다.
온프레미스 방식과 유사하지만 데이터 센터의 IT 리소스를 가상화하여 사용하는 방식이다. 특정 조직내에서만 운영되는 폐쇄적 클라우드다.

3. 하이브리드 클라우드 (Hybrid Cloud) : 둘 이상의 호환되는 여러 클라우드 제공자의 퍼블릭 클라우드의 인프라와 조직 내 구성된 프라이빗
클라우드 인프라가 결합되어 사용되는 방식이다. 일반적으로 프라이빗 클라우드의 용량이 부족한 경우 퍼블릭 클라우드에서 IT 리소스를 할당 받아
사용한다. 

4. 커뮤니티 클라우드 (Community Cloud) : 금융권과 같이 여러 조직의 업무와 기능이 유사한 경우 파트너쉽을 맺고 연합된 조직 또는 커뮤니티가
퍼블릭 클라우드와 유사하게 공동으로 데이터 센터를 구축하고 공유된 접근을 허용하는 방식이다.
```

## 컴퓨팅 패러다임의 발전
```
1980년대 메인프레임 : 입출력만 담당하는 터미널로 구성
1990년대 클라이언트-서버 : PC의 대중화로 대표적인 분산형 처리 방식
2000년대 그리드 컴퓨팅 : 유무선 네트워크 기술의 대중화로 기업 내 시스템이 네트워크와 인터페이스를 활용하여 다른 컴퓨터 간 상호작용 
2010 클라우드 컴퓨팅 : 유틸리티 컴퓨팅이 가능해짐에 따라 전 세계에 구축된 데이터 센터의 IT리소스를 필요할 때 필요한 만큼 사용

가트너 : 인터넷 기술을 활용해서 많은 고객에게 높은 수준의 확장성을 가진 자원들을 서비스로 제공하는 컴퓨팅의 한 형태
우리나라에서는 클라우드 컴퓨팅 발전 및 이용자 보호에 관한 법률이 제정되어 변화되는 수요와 요구에 따라 정보통신망을 통하여적
신축적으로 이용할 수 있도록 법률을 제정하고 있다.
```
