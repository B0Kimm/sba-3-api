OOP에서

class, instance

class : run on disk (static - resource )
instance : run on Ram(memory) (dynamic - resource;.//)

생성자(constructor) 외에는 instance를 만들 수 없다.

생성자는 클래스명(대문자로 시작하는) 에 parameter - zone이라 불리는 () 구조

instance = Constructor(parameter)

notation : 표기법 a = '1'(str) a = 1 (int) a = 1.0(float)
annotation : 주석 

JavaScript,C-Java, @static/indent(route)
constant => const, static,  
variable => let, int~,

data -> constant + variable => state

variable은 change 요소를 가지고 있는 정의 -> True의 상태
constant는 change 요소를 가지고 있지 않는 정의 -> False

state를 종류에 따라 (추상화) : 4가지로 분류, 
CRUD(create data, read data, update data, delete data)

REST(Representational State Transfer)
4가지 조건(restriction/condition)
1) CS 구조
2) stateless :
    clinet context - True
    server context - False
--------) 캐시처리가능(cacheable)
3) 중간서버 ex) WAS(tomcat)
4) URI를 사용하여 data를 JSON등의 형식으로 전송

SQL : Language

sba-api (appliciation-programming-interface)
sba-ui (user-interface)

--------------
Q. Rest인가 아닌가?
from flask import Flask

app = Flask(__name__)

@app.route('/') # decorator = 추가하는 것 
# (route  속성값을 app에 등위;/ url) => url에 결과 값이 보여준다 w/o not works
def index() :
    return 'Hello World' ---- 이것 때문에 SOAP/이것이 JSON이면 RESTful

if __name__ == '__main__':
    app.run(debug=True, host='127.0.0.1', port=5000)

app.py에 대하여
cs 구조 T -> 서버 : sba-api, 클라이언트 : sba-ui
상태저장 T -> 쿠키나 세션을 저장 안함
중간 서버 T -> 내장된 레이어 사용
URI + JSON 사용 T -> http://127.0.0.1:5000/(URI True) + JASON(False)
    (JSON의 notation; {key:value}, [])

그러므로 rest가 아닙니다. 그러나 string 대신 JSON을 사용하면 RESTful이 됩니다.

URL = URI/serach=hyper

Controller에 Rest 설정한 부분까지가 2주차 (MVC)의 종료

3주차 Model로 학습 전환

Model에서 인공지능(AI)에 대한 알고리즘 학습을 주로 합니다.

