# HTML 구조

## HTML이란?

HTML(HyperText Markup Language)은 웹을 이루는 가장 기초적인 구성 요소이다. HTML은 웹 콘텐츠의 의미와 구조를 정의할 때 사용한다.

![image](https://user-images.githubusercontent.com/55734436/104836381-ee662900-58f0-11eb-89ac-b5487fc8049f.png)

우리는 F12를 누르면 다음과 같은 창을 볼 수 있다. 이것이 바로 HTML구조이다. HTML을 보면 우리는 웹사이트가 어떠한 형태로 구성되어 있는지 파악할 수 있고, 이를 활용하여 원하는 데이터의 구조와 위치를 파악하여 데이터를 수집하게 된다.


## HTML 태그

HTML에 담겨있는 구성 요소들은 마크의 역할을 하는 '태그'로 감싸져 있다.  

가장 기본적으로 HTML은 아래와 같이 작성된다.  

```
<태그>내용</태그>
```
시작과 끝이 하나의 쌍으로 구성되어 있으며  그 사이에 내용들이 포함되어 있다.

여기서 시작과 끝에 쓰인 태그는 엄청나게 많은 종류들이 있다.

- **<html> </html>** : 웹페이지의 시작과 끝을 의미하는 태그다.
- **<title> </title>** : 문서의 제목을 의미하는 태그다.
- **<body> </body>** : 웹에서 실제로 표시되는 내용을 의미한다.  

## HTML 선택자

수많은 요소가 포함되어 있는 웹 페이지는 수많은 태그로 구성되어 있다. 그 중에서도 서로 동일한 태그가 존재하게 된다. 이러한 경우를 위해 **선택자(Selector)** 는 동일한 태그 여러 개 중에서도 각 태그를 구별할 수 있는 역할을 한다.

### 선택자의 필요

```
<div>	
	<div>
		<span> 파이썬 </span>
		<span> 크롤링 </span>
	</div>
	
	<div>
		<span> C언어 </span>
		<span> 게임 </span>
	</div>
<div>
```

다음과 같이 태그과 되어있다고 하면 <span> 태그가 4개나 존재하며 원하는 값을 구별하기 어렵게 됩니다.  
  
이러한 문제를 해결하고자 선택자를 사용합니다.

```
<div id = "contents">	
	<div class = "metadata1">
		<span class = "language"> 파이썬 </span>
		<span class = "project" > 크롤링 </span>
	</div>
	
 		<span class = "language"> c언어 </span>
		<span class = "project"> 게임 </span>
	</div>
<div>
```
예를들어 우리가 프로그래밍언어와 관련된 내용만 가져온다고 가정을 해봅시다.  

그러면 우리는 "class = 'language'" 라는 선택자를 사용하면 프로그래밍언어와 관련된 파이썬, C언어만 가져올 수 있습니다.  

### id와 class

선택자의 태그는 주로 id와 class를 사용합니다.


예시를 통해 빠르게 이해해봅시다.
