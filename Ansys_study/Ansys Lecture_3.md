# Truss and Beam Element (1D Element)

트러스 구조를 직접 제작하고 구현하는 방법

#### 1. Node 정하기

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/544d1bc5-5403-4ea8-91bd-255488707dca)

1st row: amount of node

2nd row: Node NO.

3rd row: X coordinate

4th row: Y coordinate

5th row: Z coordinate

#### 2. DesignModeler를 통해 Ansys 내에서 트러스 형상 제작

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/dd64ae99-6aa4-46c2-9933-34059514a992)

Static Structual -> Edit Geometry in DesignModeler

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/4713bd92-1246-4264-9910-855f883ab639)

Create->Point->Generate ->불러오기

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/4f089863-1d0f-4128-89c9-88b979e37447)

노드가 형성된 모습

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/2278c19a-e3e1-44c1-b731-9288ff881795)

Line 연결하기: Concept- > Lines From Points

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/4eb836f6-0413-4ed1-9ba2-bfa8ee91f349)

Line이 생성 된 모습

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/75806601-d62f-46f8-8db7-3332cb713434)

관성 모먼트(I) 컨디션을 주기 위해 Concept -> Rectangular->B, H 입력

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/24e8712d-36db-4878-8684-9f28f931e659)

Line Body를 전부 위에서 설정한 Rect1으로 변경

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/165c2900-832d-4174-b1d1-a5271190e350)

하나의 파트로 묶기

#### 3. 솔루션 제작

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/cda827b8-c6bb-4e6a-8dd7-7d87d1ebd26a)

Line body details를 위와 같이 설정

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/fc2d6d60-038c-4ba1-81d1-8597524cd170)

Mesh 생성

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/d8a75a57-e861-4c75-bda8-5d12498d7289)

Force 및 Fix 위치와 Fix 방식 설정

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/e8989df2-37a7-4f9b-b2c8-c5d2145baaf3)

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/962ebeea-a38a-4c08-841c-ff3e134c158a)

Vertex로 설정하여 지점 설정 후 Force Condition 주기

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/7a2466a1-989b-4212-8e25-13a775102dfc)

Line Body가 Beam인 경우: Bending이 있기 때문에 Beam이 Bending 되는 것을 확인할 수 있다. 

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/ab65716f-3f50-429b-9355-4194616328af)

Line Body가 Link & Truss인 경우 : Bending이 없기 때문에 Node의 위치가 변화하는 것만을 확인할 수 있다. 

