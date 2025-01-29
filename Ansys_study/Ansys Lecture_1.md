
[[typora-setup-x64-0.9v-free.zip - Google Drive](https://drive.google.com/file/d/1UmDNSUdOqj_w2y3YWqwOY-gAXmrvtxKO/view?pli=1)](https://drive.google.com/file/d/1UmDNSUdOqj_w2y3YWqwOY-gAXmrvtxKO/view?pli=1) 타이포라 다운로드

# Ansys 무작정 따라하기 1

Ansys 설치 후 Workbench 실행





### 2. 물성치 추가

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/9de43859-b8dd-40b6-bc98-ed27beff4867)



![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/6fd5c298-4594-4c43-a81c-99d10648115b)

Engineering Data -> Engineering Data Sources -> General Materials -> Aluminum Alloy (책 표시가 뜨면 추가된 것임)

#### 기계 물성치 추가

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/ffc3fe08-8331-454b-8e69-ba2954568355)

Linear Elastic -> IsotropicElasticity 드래그 후 추가->Young's Modulus 와 Poisson's Ratio 추가

물음표가 사라지면 필요한 성분이 모두 추가된 것

#### Density 추가

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/955e5a24-6dd0-4748-9580-4ed1524b214a)

마찬가지로 드래그 후 추가

#### 물리량 가하기

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/d4c79dc2-632d-47dd-be32-12586285a49f)

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/6a9c10e3-ebf5-4ed3-a766-c7726939ed5c)

힘을 가할 위치와 Components를 설정하여 힘이 가해지는 방향을 설정할 수 있다.

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/03427451-ac1c-4791-ae27-bc7ff99112da)

Mesh->Body Sizing 에서 Mesh를 잘게 쪼갤 수 있다.

#### 물성치 파트에 추가하는 법

![image-20230831152427174](C:\Users\user\AppData\Roaming\Typora\typora-user-images\image-20230831152427174.png)

Geometry -> 지정한 파트 -> Material -> Assignment -> 변경

1. ##### Part 모두 Structural Steel 일 때

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/cf59154f-f0da-4267-bbd1-72a6b7572573)

##### 2. Part 모두 Aluminum Alloy 일 때

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/1420839c-eeb4-46bd-910b-ff36d1b802bd)

#### Path를 이용해서 부분적으로 해석하기

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/8570de5f-b4b1-481c-92db-a611cd58bf1b)

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/f5f14263-739f-4c24-8bbb-8dddca02937e)

Edge를 선택한 후 Coordinate 정하기

아래 부분도 똑같이 Coordinate 2 정하기

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/0f8eea76-4b66-4448-9cdb-e55582542e29)

Construction Geometry -> Path 

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/1259189e-281a-4f1c-9fc8-447885ab6463)

Path 입력

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/231f8684-5ee9-4815-a9f5-5a181e961462)

Scoping Method -> Path -> 설정한 Path 추가

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/ec6ac1eb-561d-444f-b834-0b2d0dc0f187)

재료가 변화한다 해서 Stress 는 변화하지 않는다. 왜냐하면 Stress = F/A 이기 때문에

#### Remote Point, Force

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/20f75fb2-45d2-4393-8a40-0858ac7c9b43)

​	![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/6d7da2ab-02ab-4c30-a350-ba295ed782bd)

두 단면을 선택한 후 원하는 방향으로 얼마나 띄워 포인트를 설정할 지 입력

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/90605318-fe41-465b-8541-bf7ce61780ba)

변경한 위치에 힘을 가하기

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/934112d1-5ea5-4bba-b7af-11218459fa0e)

![image-20230831163318765](C:\Users\user\AppData\Roaming\Typora\typora-user-images\image-20230831163318765.png)

결과값 확인

#### HW1_1

 ![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/4fb47c7c-efdf-4934-b3a0-5ed730f1edf9)

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/df433356-aeef-4729-98b6-d96eb05b8ebf)

#### HW1_2

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/5add7d0a-2533-4eed-b983-cb40a8582f36)

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/d19e323d-6d7b-4b12-8b6a-f759ab60ab96)

#### Tetrahedrons 으로 Mesh Sizing

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/3a516127-ef94-41f1-8358-4a8f86689666)

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/c5fb0f04-0dbc-4f8e-b65e-150047458bfd)

만들기 쉬우나 Sizing limit이 있어서 버전마다 Solving을 할 수 없다.

Mesh Sizing으로 이슈가 생길 때 Tetrahedrons을 사용하면 쉽게 Mesh Sizing을 할 수 있다.

결과 확인

![image](https://github.com/AnGyeonheal/CAE_Ansys/assets/118132313/ab8f53f6-339d-4179-a692-412e0adaeb3f)