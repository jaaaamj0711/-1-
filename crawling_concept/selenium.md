# selenium 내장함수
동적크롤링을 하기 위해 필요한 selenium 내장함수에 대해 알아보겠습니다.

```
driver = webdriver.Chrome('./chromedriver')
```
먼저 다음과 같이 driver를 정의하여 줍니다. path설정을 주의해야 합니다.

## 1. get()
get() 함수는 입력한 url 주소로 접속하게 해주는 함수입니다. 사용법은 다음과 같습니다.

```
driver.get("url 주소")
``` 

## 2. find_element_by_ ~ ()
이 함수는 정적크롤링의 find()와 비슷한 역할을 하는 함수로 HTML 요소를 찾는 함수입니다.  
find_element_by_는 종류가 굉장히 많기 때문에 ~로 표시하였습니다. 많은 종류 중 몇가지만 살펴보도록 하겠습니다. 

- find_element_by_css_selector
원하는 CSS 선택자 조건을 만족하는 모든 요소중에서  첫 번째 요소를 출력합니다.  

- find_elements_by_css_selector
원하는 CSS 선택자 조건을 만족하는 모든 요소중에서 모든 요소를 리스트 형태로 출력합니다.  

- find_element_by_id&.find_element_by_class_nam
위 두개는 id 속성과 class 속성을 가지고 있는 경우 사용하는 함수입니다.  

- find_element_by_xpath
XPath는 HTML 요소를 찾기 위한 적당한 id 혹은 class 등이 없을 경우 사용합니다.  XPath는 다음과 같은 방법으로 찾을 수 있습니다.

![image](https://user-images.githubusercontent.com/55734436/105672074-27248480-5f27-11eb-992b-1588796a9cf8.png)


## 3. click()
click() 함수는 말 그대로 HTML 요소를 클릭해주는 함수입니다.

## 4. send_keys()
send_keys() 함수는 HTML 요소에 직접 텍스트를 입력하는 함수입니다.
