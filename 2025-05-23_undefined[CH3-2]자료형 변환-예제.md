
### [프로그램 3-8] 암묵적 자료형 승격


	> 💡 암묵적 자료형  - 자료형이 산술에 맞지 않는 경우(불,문자) / 자료형에 맞는 연산자 없는 경우,  
	>                         컴파일러가 자동으로 자료형 변경


	```c++
	// [program 3-8] , p.94
	#include <iostream>
	#include <typeinfo>
	using namespace std;
	
	int main(){
	    
	    bool x = true;
	    char y = 'A';
	    short z = 14;
	    float t = 24.5;
	
	    // bool → int 자료형 변환 
	    cout << "type of  x + 100: " << typeid(x+100).name() << endl; 
	    cout << "value of x + 100: " << x + 100 << endl;                
	    // char → int 자료형 변환
	    cout << "type of y + 1000: " << typeid(y+1000).name() << endl;  
	    cout << "value of y + 1000: " << y + 1000 << endl;             
	    // short → int 자료형 변환
	    cout << "type of z * 100: " << typeid(z*10).name() << endl;     
	    cout << "value of z * 100: " << z*100 << endl;
	    // float → double 자료형 변환
	    cout << "type of t + 15000.2: " << typeid(t+1500.2).name() << endl;
	    cout << "value of t+ 15000.2 " << t+15000.2;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/f4afcf66-d7ce-475d-a25e-bb775ebe0f20/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466ZVQSYBS3%2F20250523%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250523T113828Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEDMaCXVzLXdlc3QtMiJHMEUCIQC8Y%2FVIJPvP8thpKLTUf5aDyFGqErGU2U385t4YwQOjAgIgV9rqlyez6rL1HZZN475Cxz%2BXDYTYPb8WohwP5dnrBfAqiAQI7P%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDKkSuA8ewglhHYbyOircAyrXReOa38CMegaGikaTheg6uDq9S5eijut9sY8fNVV4rglH4XHoq8HfzBz4AqiOXBKk7EsqWOKrHveFtHCsj5SZEhCqb3Bqg0lDjkRHtL9SrHbom7%2BMZWLCmK2%2BX4zd6XQ8ZpEBHFl9mk%2BVLh8If6i2yZAbtFBrqaKPr3heyzVAymDw5UwWFzoWIjcKLHAIwps5ZE3%2BizPKcfuZDVGzIQepM5ETYzb1nITnpc00waMleDDuuwkCWwaa2pXQY4fbLlEaZ2lxw6tTZL%2BWAnOUoXp4UM7J%2BJUCbsXJgX3c3IZQYNRsDGDYnrrp5iEDi0%2BIu%2BFDQ2h9pvpE2UIS1WL7EORrem1rsQmwMmlYj2CY3RRy9QMIcCSYxSQN7AtkUTmYF81DOoo%2BX7gPQS4tTxIKVPH7WXLTyjvunv7UwX%2FSj6CuSst6fC8IVe4TIsIT3X2U6Om8oDGlbSmFJ8hei9e5hIRDZu3Be81yXazFRtYxtP63gSeWU%2BrXay7nkVa%2B9U7n2uAlNS%2FlMAQs13PTD6TJuvKAju6Z0%2FfD6T1KUQ%2B55LA9ZHwkcOZVZ6Tp83toMUGWbDfiM0b581s6LLy4tg7WxOT7FWvWWlw2UnmNYfRB5JW7T5MTOYuWn2%2BSz2PMMM%2BpwcEGOqUBtdSp70ugWH4ybFtMziep%2FQZ%2FFAc%2F4J9ha%2B0gyts%2F42x%2BHWmCex1kg9rG4UyAJlS5AgxAn3jXSC790QNKrjFF%2FRG34IoVqjHTgHguh%2B%2Bs7sF0h9%2Bab%2FAJ5bCkRgwu7h0Fc%2FzYoYx%2B2sVY0aBiBg5GMcFqCrUQYVgCZubBL5U7FwJX6nWbmUmJFVpcg1jZ7GZroL6cpVk354QQV0v1DyDA4LvZQcMB&X-Amz-Signature=7f5263958b440f393e751cb218dd308357055e8e85f28433ed13294b99d53f51&X-Amz-SignedHeaders=host&x-id=GetObject)


### [프로그램 3-8] 암묵적 자료형 변환(부가 작용 없음)


	> 💡 부가작용 X  - 암묵적 자료형 승격이 이미 일어난 경우


	```c++
	// [program 3-9] , p.96
	#include <iostream>
	#include <typeinfo>
	using namespace std;
	
	int main(){
	    int x = 123;
	    long y = 140;
	    double z = 114.56;
	
	    // x + y의 자료형 및 값 확인
	    cout << "type(x+y): " << typeid(x+y).name() << endl;  //long
	    cout << "Value(x+y): " << x+y << endl;
	    // x + y + z의 자료형 및 값 확인
	    cout << "type(x+y+z): "<<typeid(x+y+z).name() <<endl; //double
	    cout << "Value(x+y+z): " << x+y+z <<endl;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/29751a73-ea65-427a-8341-6d2934edba6f/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466ZJKKHYKY%2F20250523%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250523T113829Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEDMaCXVzLXdlc3QtMiJHMEUCIQC3rFZfzeUTsp%2BA6W5a%2FCjpdSIB2uBSoG4hKsnJPhJuBAIgGbotDnURQGj5qCUjIymTHJte43ufQ2ZO06FaTZ2PkIoqiAQI7P%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDM5JlYdvlFa%2Bqm%2B4dircAygYu5q%2FMvhAAW2YaxPYro2f3jKpRQ9GhY4tt3YVJReBSPzZFATeTKxYEtJQSkxrQ5gAR9kEtSaICvQL8TJGK70fDZ31RO5oRJka7wtxBwxJBgIAchvGWUbAhXf04N0F%2BmaiqmYAWbKpeYm9660XkXFv%2FuvlF4iGi0NZKGaJwNT6clrFdqfvlOqzU3Y4dZmog7Zk0qFBk8%2FLWETmdWVAxSZep4PD2Ybjpf1olg8rO8hedOx86kliU%2BB%2FJpLQgbaDOU0EDG%2FcgTyUVQf4CzhD05yszAtrjiu5u%2FTFpCNBqjVUAluBgPcbUt8L85AsjDc6aW2EJ6nUlcpPgiUVllNS0VwTi29uj%2FxB%2FRtX69I8%2BvgwuqyRFDhtBn3CM0vpCezKG7MFk3RBvipPmJDvZPqXiQdN84AI99atn%2BJDDL4ymSGPG0SmnKYTSoLOQtI0GKWH%2FDPkDZCv8ReO1c1EWc2it9JotbRpR9V92oB8c8kSTcQRsDinxiFmlIhTTtmk0VxZTr1NYNpzgjB9Ye00b6QNAKcxMbvA9OY8yy8K5RzNbWCoiyaq8s3LURSoaBfGLuMRE23SIwG%2B2trq6io7cuRhJXYyoq96bfBLwQXHpcv4TpyK%2BWmueXWGPtRR5GUKMMipwcEGOqUBO7EpmczbYpiYNlwJ1bDWfRu%2F7Wyd5rDo3su71TB0Mfyzr1xe%2FSFLeGBv9dcOruAr7RR5bBejICJrQHe7Sy51JN5AA%2FLq5Ghe9c%2BD9y2aod2L8%2BTuBfzjpdz7LELKYmeMijWTSamk0S%2B4gOALmpKgMRLUmEKQOerWSUl%2F3h9A%2Fd1Q0I48%2FPU%2FB8v4l5jVxXKJogGkiK4zjvMJxDdjvqZcyRFk426w&X-Amz-Signature=bb7da46c428b6de6bc1534afe4ef7e4c7bfeff374c79b4c47cfcc541f61f3e40&X-Amz-SignedHeaders=host&x-id=GetObject)


### [프로그램 3-9] 암묵적 자료형 변환(부가 작용 있음)


	> 💡 소스(값)을 대상(변수) 자료형에 맞게 변경하여 자료형 변환


	```c++
	// [programing 3-10], p.97#include <iostream>
	#include <typeinfo>
	using namespace std;
	
	int main(){
	    int x;
	    double y;
	    x = 23.67;
	    y = 130;
	    //x의 자료형, 값 확인
	    cout << "type(x): " << typeid(x).name() <<endl;  //int(i)
	    cout << "value(x): " << x << endl;               //23, 소숫점이하 생략
	    // y
	    cout << "type(y): " << typeid(y).name() <<endl;  //double, 자료형 변환 필요 x
	    cout << "value(y): " << y << endl;               //130, int값 -> double로 저장
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/229dca58-46df-4b0b-bd6f-a8b75b131e52/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4666KRPHMNC%2F20250523%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250523T113829Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEDMaCXVzLXdlc3QtMiJHMEUCIQCKXzv9PO1%2F5umJOrwy9hKfa6xIMqPPtwtBGbzp1ibCogIgA6oGTRPi6z14ObEDuwoifjw8acvS%2BjAOOLy3IecA67gqiAQI7P%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDNtIswFpVRCsneMd6CrcA4QQ7CD8OrYPzJuHYXfdRlB5Ipl0lvGTB2FmodOI9%2B5L%2BDngBVt%2FHte21DOlJ%2BcuZfxkrK7VxGTiAmRwuMOGb%2FGT0VVG8oMfEro3o2hsJhLB3XBbs9f49P6EJsb%2FRqck4cSmoBau2E%2FrTJgdOWTuqX6pusSe98Q6CJOfb%2F9beUDfIZXOk553ZsPUiUbJtdXKcDEFFLBs5JVk9oeuBfW%2FjQdkc3NcF5ptSclqzEMMi5se9Ikj3KKug89FHIB%2BFZ3hqPDZ8hRbZMXGwQW6To4p7M1lVFAmbS9QdpCYSkwNA68rG7Wgn9gQnew%2BkLrQR03x0yzZmZI%2BAI4v3%2BRnjeH%2Fqp2zPjQRUb3fnz4FRF0WTEHorGEPdZXzhuRM1UaLsXSmyMTGA8Ex%2FydgK2pPzqohF3tOUqBQnQVPNCOv5GH97VmLTzOxJKwtV%2FBC5KzB7%2BZpOhSCBRRsPtUF9bXr6NkBz4wD3K29TvU77i3UChTs8ncdP4hz%2B9DtmW92SPeSAQvoFGvz5jYbACG%2Fo2XFbsQn5%2B6Lix8JMqh8JqG85E%2BEhlnP2bc4qG5r9MYQB2QlZ4v9TsqL5NlFhQILgcJM%2BzCCLexYstsgxK0SIuLKok%2Br4X0NKwwA6Wps7BHK0fAjMOCpwcEGOqUBLKgHcxcjVtJTf%2FXJKk5aHPstjhzgz4qcV0smhh%2B4BqRtl0PArKtGhJm%2B7r%2F%2FSvYNr1mTCbBhHUblHj3MJt9sdBGO98ATDNHhEGkZ37IBBP5k5ElIOQDTakqoW7rQMP%2FmtzXlSSmYltSJqzDTBWTKkxoeI5ERKasfJpDtvB6WYUfxdL4K255KLmC%2B9H4wdEYqrd2hD2ISRtPLeY0Nx0G73Q2ovnlF&X-Amz-Signature=f2644f908f1a59b8e6d28e2404cf9076d326b2c53169fd228e905ca14c6977bf&X-Amz-SignedHeaders=host&x-id=GetObject)


### [프로그램 3-11] 명시적 자료형 변환


	> 💡 `static_cast<자료형>(변수명)`을 사용해 자료형 강제로 변경


	```c++
	// [programing 3-11], p.98
	#include <iostream>
	#include <typeinfo>
	using namespace std;
	
	int main(){
	    double x = 23.56;
	    int y = 30;
	    // 암묵적 자료형 변환 활용
	    cout << "Case - casting X: " << x+y << endl; // y가 double로 자료형 승격될 것
	    cout << typeid(x+y).name() << endl;          // x+y 자료형 확인
	    // 명시적 자료형 변환
	    cout << "Case - casting O: " << static_cast<int>(x) + y; //x의 소숫점 이하 생략 → 정수
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/e149d3c4-de3a-44eb-8c0e-75af1c0c9ee7/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466XQ7WYXL6%2F20250523%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250523T113833Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEDMaCXVzLXdlc3QtMiJHMEUCIQC6wKTDXzHmIgra7D%2Bm4KHFunNhBUh%2F%2FNNSui9lzL3iIQIgW67%2FXtstS%2FSk2IT0NziBpUfEuIfNC1A0xcn%2BB1pS4IoqiAQI7P%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDKmY%2F9OnECfL6T%2BwQSrcA1oTigo%2BTOjOic765J3p8LoNpvtL%2FetA9ZWxGlD%2BwFhqrQf6TQCGfXjxyTOQgPzl%2F8gMhaRGsRCm4BQMBsxwjKA%2B%2BcvARIg1%2FkM77MfiaLy3Osp8B%2FArblclYj1Rjqr05T6QA9MW8b8gM0cu9gfvtluf5149JFbncjQrUheLvwx33IvOaGtgOunhdgzFPX6e8z%2FERmxK39MptCy3fUmRzBsDF6bvjb9zHBj568ERzgiGEQy0f48p35I%2BdXCxcP50F1t9VxYs45Yvu8GHyybXAKfPMlPOJAfjch7IBtTbtD1id6mOeRAKLZTw4gSkjtkR3PGWVmBYjVa6DSn0Z8rPJ%2FnIGz%2BxE7rfU2XBgt8t0q2DZzkH9SQ0Ka2l5fhDFZs1QYmpqfRU%2FoajzFEGYdxxDuHrk54R96kU89vdvBVtaeyfxbDtnPZQlpGqOLw%2B4OHeEudwZ8BlUIp9awO%2BGgr2Eivq29%2BMz3Cld4UKdswNF4qA%2FOm%2FFTFfqD9BXC153QErarlYCBvMKuybHaoF%2Fs7u1CXrDY6XukPPI7Mka9fQACJ9C6qQXZw3CnwOlzF5lzs3W9E%2FccWZFQkcqVaLMLsgHaf1B9Wel7sE0n6pmMUU6%2Focc5snIMmnT2fKCUTaMNauwcEGOqUByila6%2FSyyopN%2FECBYZhis0dK86NkBwtAQ1czKeTUVGRkBbgwuCbEyufjCcl2CSRPiOGyHsLWlEyprkqtrSQc95gM4WUuIOhI4GLk3kJ9Z4U1IKRJIwdUCmy3Nggn588G2%2Fxs9LHl4OSIOqrB4AKf6NpbM9CvCRfT0Heb2YFoK6TXux%2FP1xuidMaFyYlJOP9yPBYOeR2Pzv9Cb7ZAVtj8ywvrDGcg&X-Amz-Signature=b4861bab69f34c171db2e30f3e8e097df31a3c1eaafec51b4f65ad5f01ecc3f0&X-Amz-SignedHeaders=host&x-id=GetObject)

