
[CH2] C++ 프로그래밍 기본  


> ### AND 표현식 사용  
>   
> - 두 피연산자가 모두 true일 때 true  
>   
> - 2가지 조건을 모두 충족시켜야할 사용


	### AND 표현식 사용

	- 두 피연산자가 모두 true일 때 true
	- 2가지 조건을 모두 충족시켜야할 사용
		- ex) 값의 범위 지정 (x≤value≤y): `(value >= x) && (value <=y)`

> ### OR 표현식 사용  
>   
> - 두 피연산자 중 하나가 ture면 ture  
>   
> - 1개의 조건만 만족(둘 다 true도 가능)하면 될 경우


	### OR 표현식 사용

	- 두 피연산자 중 하나가 ture면 ture
	- 1개의 조건만 만족(둘 다 true도 가능)하면 될 경우
		- ex) 값의 범위 지정 (x≤value, value≥y): `(value <= x) || (value >= y)`

> ### NOT 표현식 사용  
>   
> - 논리 표현식의 값을 반전  
>   
> - `!(조건문)`  
>   
> - 부정 연산자(NOT) 제거


	### NOT 표현식 사용

	- 논리 표현식의 값을 반전
	- `!(조건문)`
	- 부정 연산자(NOT) 제거
		- 가독성이 좋지 X 때문
		- Ex) 종료조건 = (temp < 5) || (temp > 30)

			계속조건 = !( (temp < 5) || (temp > 30) )


			               = (temp ≥ 5) && (temp ≤ 30) (∵드모르간 법칙)


### [프로그램 4-9] 윤년 확인하기


	> 💡 윤년 확인 조건  
	> 1. 400년으로 나눌 수 있어야 함.  
	>   
	>   OR  
	>   
	> 1. 4로 나눌 수 있지만 100으로 나눌 수 없어야 함.

		1. 400년으로 나눌 수 있어야 함.

		  OR

		1. 4로 나눌 수 있지만 100으로 나눌 수 없어야 함.

	```c++
	// [program 4-9] , p.151
	#include<iostream>
	#include<iomanip>
	using namespace std;
	
	int main(){
	    double hours;
	    double rate;
	    double regularPay;
	    double overPay;
	    double totalPay;
	
	    cout << "Enter working time: ";
	    cin >> hours;
	    cout << "Enter pay per hour: ";
	    cin >> rate;
	    regularPay = hours * rate;
	    overPay = 0.0;
	
	    if (hours>40.0){
	        overPay = (hours-40.0) * rate * 0.30;
	    }
	    totalPay = regularPay + overPay;
	    cout << fixed << showpoint;
	    cout << "regularPay = " << setprecision(2) << regularPay << endl;
	    cout << "overPay = " << setprecision(2) << overPay << endl;
	    cout << "totalPay = " << setprecision(2) << totalPay << endl;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/d7887bca-a1bd-4a0f-b62d-092d9802183c/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4664CAZU5TQ%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044651Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIHSGayZB8pwZ5CX3fXZ8bEAZ0J9C7QEv9UX0LR3v7vxKAiEAzIhuxZGapvlirFITMZytMkB3D4FaLhoZy6ioXCqJKbgqiAQInf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDPOUKcsIRyZtMtA4iyrcA8LugjQ2n7SMw7X7aGNwIHeW4UK2FcKJMUZDD53ltg8bwD6Bn6ii4pwIcNvPSnrouLRopQxz1aDDsEOM3Nryzb4wVvYbJTKhWw0J6T6gDXhnjSU%2FSajnyiLK1eYTd2TS%2BxW66q7uZ4AE9%2B04pncbJUlFmjFmrYaAmZK%2BK37XsOJ7M6OPUHxb9tv1eoFT96ZTmLUCHu3f38O3HOIoEYY%2FRHnS6e%2FTf9HD8T6aBZCTaqEljYqlGr3Pq%2FUSg4WGm2YLVwWsO01Xzyrc5YwSdoQTBZFz5jtQDohNWcR1ZDDwBbZUgX3nTr2T5aPplPLv7R1FoGOuWkaDJFUvR45srp%2Fu6YYTPjmPBVhE4r%2FtWJW6y8%2F7eLEn2kt2zb2c3JV7e1mebnFfBa7nU7A4kJivs0LHYjkeEGkeZqsaEAmcP8pWQ9d4Spd1pD9tY5TMMVncIdiP9KpgYwkPXC4vWtQolICAo47dxcEF9BQAabPzzQC%2Bx8bTneszBBckZwADCrUjHGoUNHnHlfHSZFwHIuotNTqfqtVfEX5zHJ3KmSCaNFXzlRctDJSrczhMptuCKP1xBB43JRTXab54dFGT68JIUsDSFUNA2uw9ohctUZcQiIIDCvLNCj2Veubkdl81EBX%2FMNjd5MEGOqUB%2FHzWDG8kwJyjily1O4%2BQH8P370wX3ENzw%2BrmKT%2Fg96qUa5sx%2F3eUt%2BJJbRq%2BoWSZE6MB8XpQIEAc0ErTPx%2BTvRcXuxV3HyEpTmMOUugxKDTaO4nLCYHjlPiVLBgYMMkvYS8EredQXCdBHa8D00Q7c1jEEbnZgbQv1UrTLqWfBouFV8ILwMpC6aG%2BWIfDPe5T0oO1SuLLELCi29JdkDKfBV9%2Br0y0&X-Amz-Signature=0476bfbb76d98195c46e4fa78c3324ab9b72ecaa83b12958720e182f9efd71ab&X-Amz-SignedHeaders=host&x-id=GetObject)

