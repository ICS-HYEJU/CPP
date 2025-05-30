
[CH4] 조건문


> ### 조건부 표현식  
>   
> - C++에서 유일한 삼항 연산자  
>   
> - `조건 ? 표현식1 : 표현식2`  
>   
> | 그룹      | 이름      | 연산자 | 표현식          | 우선순위 | 결합방향 |  
> | ------- | ------- | --- | ------------ | ---- | ---- |  
> | 조건부 표현식 | 조건부 표현식 | ? : | 조건?표현식1:표현식2 | 4    | ←    |


	### 조건부 표현식

	- C++에서 유일한 삼항 연산자
	- `조건 ? 표현식1 : 표현식2`

	| 그룹      | 이름      | 연산자 | 표현식          | 우선순위 | 결합방향 |
	| ------- | ------- | --- | ------------ | ---- | ---- |
	| 조건부 표현식 | 조건부 표현식 | ? : | 조건?표현식1:표현식2 | 4    | ←    |


### [프로그램 4-14] 조건부 표현식


	```c++
	// [program 4-14] , p.164
	#include <iostream>
	using namespace std;
	int main(){
	    int num1,num2;
	    int larger;
	
	    cout << "Enter num1: ";
	    cin >> num1;
	    cout << "Enter num2: ";
	    cin >> num2;
	
	    larger = num1 >= num2?num1:num2;
	    cout << "The larger one = " << larger;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/7d50b2ec-fccd-47d8-b047-2bd124968907/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466XIDRVFXS%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044746Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIQD6%2FBwFR7m8Fo7qzgaZtc4Cp%2F4UBuX3t2uDubuo%2BLCFBAIgQd%2FrnmkF6cspk5aDW1oGcRhn%2B8MMA%2BCXuzP7kiUdSk8qiAQInf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDCbEZp0Jh2sTJtX2OircA0pYBOrmyxyhnROvYVQp6KOnb3TQ0DDE3XMmaSIDY1VPgQUafPm6WACzrhu1hZEo6BfRzpvfO8vlY7bgb6YDarztGrUyz3F%2B%2BOgNfZ%2Fh5Ak7%2BXSXVl5UQgsQmaLjWcVtNHMtxqyzwElPhPDDc1WhsSzKyg5G%2F1%2FyMj0ZWMCPUMg0PY5YBpunRlQ8Ht4CUh%2F5ovNty%2FKUEtpNdQHtchx0kGVzkeheU%2FJCbaBjbcemWCUZ11ksEIqA%2B7ythaC97m8d%2BXXpi3k2YpKpNXunn26fnSeSRKg2bmwD3TCh%2F0dr%2FjCPUBjJo5pvtt8cNtAx8ruOAB%2FsEMiNM6LrTM%2BLyV7BGhvzRzK%2B1VvtMsVrzYe3gEVYD%2BQB%2F7HvJZSKxZTKA7%2B2D6ht37uFV4RHZLpnRConB%2BnMdBImXhSC1dhSpPEBlULcSzUMGlLdjTo5bL0HnuJq5DojiJdwlqeMnxF6qL4PUzQXWrLDT89FydY44Y3ZtTfROlgrtpJiBbI35Sodd3Dr8BTaQFaXmUeSueAVXA2Bwmj7QRCz6nzQ2ixqXSJ9hSe4SV5UYaI3NIY7zdN8j0P%2FYQviSUr0At7YSvVwuMhIztaFP3okBanm%2BWZGZBb1yQm2UN9w%2FGZuT8huMpXBMPLd5MEGOqUBKFMxX7VbRW%2BWpFpqRENimWw2mzEkeAdsuk9kf37dRgs6lhqHyu0qGa9jOWuKF7Iy7DYhwGOHuNPo4yRsjRaKo2OhSJI23ncHGmX4qmgxydehVKBIJVPysnPxqmIUuTeSWAMjyWdxQ%2BsyCCJrExjs%2FbKrsUeT1BQz1ElX4zYRrD0DcYb%2FqCx7neH3OZ2ionsl4Gq5BaRe6I77hT843LyzRpPtljii&X-Amz-Signature=16354da37e5bce0ba59f2fe35554372a298dbaf31c9b1b65c2aef936f0563dc7&X-Amz-SignedHeaders=host&x-id=GetObject)

