
### [프로그램 4-2] 초과 근무 시간이 있는 급여 계산하기 


	> ⚠️ 부동소숫점 값에는 일치 연산자(==, !=) 사용 X 것이 안전  
	> - 시스템마다 부동 소수점 저장 방식이 다르기 때문  
	>   
	> - 정밀도 차이로 인한 오류 발생 가능

		- 시스템마다 부동 소수점 저장 방식이 다르기 때문
		- 정밀도 차이로 인한 오류 발생 가능

	> 💡 `setprecision(n)`  
	> - `<iomanip>` 헤더에 포함  
	>   
	> - **출력할 자릿수(n) 설정 조작자**  
	>   
	> - fixed의 유무에 따라 출력범위 달라짐

		- `<iomanip>` 헤더에 포함
		- **출력할 자릿수(n) 설정 조작자**
			- 1234.57 = `1.2e+03` 같은 과학적 표기법 방지
		- fixed의 유무에 따라 출력범위 달라짐
			- O : 정수부+소수부 기준 다섯자리 반올림
			- X : 소수부만 기준으로 다섯자리 반올림

	```c++
	// [program 4-2] , p.134
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


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/fb288af3-a5b3-42c7-a587-b23a50b1ee0d/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466R33DB3OF%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044602Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJGMEQCICTzAPRq9j9hGVlGRlo9cKMqJMwAcjj5gLEANF6TcV3uAiA3avsuaINJpy1UpGSEVwCtWIesp%2F9Q0%2BU4XV3TIM0m0iqIBAid%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAAaDDYzNzQyMzE4MzgwNSIMOPXr9crr418%2FuqOMKtwDl%2F%2FZxsCJUrLCinpTKJCMXRAfDd8006LSg5%2BUHbmZDDoY77JjLp8MueZk4twVb5hqm2zZCsNcy%2FYHgpwGspXaSXXgSUB%2FLfEqSSqVBsxSGeez7K0iKjFYFQ8MbItiyxas5hFEk5C3N6k4og3C4qsj%2BnkitW5bGTuuPEdnbIHew5VbOP6cOJCJvavo5QlFHLlBxSXOnJ6pDH0ssS07VhdAV%2BEQyT2SHX%2Bsw3TjxF44%2FaEbq4egraWWaiSwQ77RGv2hH9Yhmv5ByPvd2M7RGsqYhXtnrFYUKlA1sZti0eqBL9n3neYsAvJzzu9psWmH5ADA%2FrlGS7sJLzbe2J03gAkpS%2BRjeNRhBOZSf358AKJ1YSV3VpXzxtkb7FQBkLTcVUd0QAjD3Oqx5m%2BQsGaRasAuAYpO42ukuk%2BJqJL5fdWJeA55BsH4WGt9wpDpcT2rA6nyjfOfWPFOTUTdcnwrZqpGKv3QiLDnvH2phi8J72rZZbI0AxABUhfNJpp3EyXKwg%2F2sLGU0Eys1hbg4%2FZGpCl1U3YopKeOXBKdrzXBlceiRhH9mB04NXNghTRBj0l86qAY9iasJcVKEDNSwr5t2uR0fzDSKymH3O6eC%2BccEG8oNzJ2VKFXzQ8EzNETzeow9d3kwQY6pgEmkeDF9JtNYlZ0vvQyqoL7VD8ziL5KQfeqg9a%2BeIMEdVk%2BcllniiEbpCJfvYxf%2BDfFnOLVZhPgSGDyICBtxlIJBdd4Cfr5WESso6SjT4s7aBeDgT%2FsGY0mYNjg7jsPe4c4U2uGniX4VgyG%2Fw46gg%2FQKoDdYqSpWFAU7mw41V15M8vih0TFz%2FrFkJBiDlpMtJMosLErm%2FzK7xD0kg9Sad7HuLJfXajs&X-Amz-Signature=8e8b8f37754f204e0bebc5d289388d2abb00e7326210db28d71f5f0ab9af4095&X-Amz-SignedHeaders=host&x-id=GetObject)


### [프로그램 4-4] 두 숫자 중 큰 수 찾기


	```c++
	// [program 4-4] , p.138
	#include<iostream>
	using namespace std;
	int main(){
	    int num1, num2; 
	    int larger;
	    cout << "Enter num1: ";
	    cin >> num1;
	    cout << "Enter num2: ";
	    cin >> num2;
	
	    if (num1 >= num2){
	        larger = num1;
	    }
	    else{
	        larger = num2;
	    }
	    cout << "Larger one= " << larger << endl;
	    return 0;
	}
	
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/11e0aa89-4a28-44e3-a7de-44a62371e233/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466Y7HRROOY%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044614Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJGMEQCIEaUI75PrIJyvnobgXAnopCXKtIW8BiV6KmyyK%2BKS3c5AiBJ53xowXqw8I%2BAurLaYaXranfvlvy9bYvFHkEwMTMlvCqIBAid%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAAaDDYzNzQyMzE4MzgwNSIMjd5DIE6ROAP4WQ8WKtwDlJRHHJN8dmJ9dlul%2FPnV%2BJfGBHhg8Z39XzevsdGAQ8ySx4J3BGugCIAU4uPBoZNfKHrLfLJYSZjvxioNxcDN92pRFpMsZFZ3OayKzavHC4KS9G2vvk6g9IpfdpmkumJu%2Bqks8R4TjEQDLgcLbmS0zvEj0T%2BzQS0S%2B7rZoZiMjeL%2FORx39MQU1Lz2goWtpoNIb%2BEqUaU30FRGzoZapjkc0kpMCxZVI%2FWNvWYlIANehsqFTzwXolPGo3qxjyldMrCYvJlmIAP0s1zy43zJtcMlQnsCMtRhP0At9j5t67yXDP7w0I%2Bksf1WLwcFGkkrwXZs8%2F4DxxDqiAAZ8KoyZ%2BSseIkAfM6NhJsnfAG2qrqDYrwbmfpwP9nxu6cx0oL2Kyu9uVarojHfwRSyr1G6yLqgESlJY%2B5LqX3R3gtYqReLSwH8PQJ7c4WirxSngqTYfQiDChkAA7ebmnRL4xJZERwjkzgG2xELuZg7WVAEs41m15QDBibPAHe2rrqn0FTLqzb%2F%2F683QRiP5NUaxAYMznimaOSAG3%2FwL1lxBlK2MlU6k4Z7rPJNo9b890wGlTrh1SJVwH3hgE9s28nw26belg9lYff47Ia%2FIcOah5g2nDQoG7OJDTF%2FW9xeEhj78scw1t3kwQY6pgFoLYZE%2FC%2Bk76dzBhNDEhI8QIniu%2BFQATFOlDLUdbrKm6RHOJl2nQGZGlb1ICm6DLWzIjLiikTcfSga0usF%2B89fEOKWRJ4qkOZgHoAWCDxLQnaGjSLdnzHeI%2FLsqoCWu5OuE5VY%2FqWL%2B8PlVtIEi%2Fnn9RJzS%2F2CRdIblfLg5v5DZhoFv0sLbhCEMNNeSjNVSmtNh%2Bk5YPbK6BwOBkxbbUYWFb9Q%2F1Kt&X-Amz-Signature=49ff1642375d9c33c6262955d883dbdc30d3e5d711fa8955bad6b1b6920670a9&X-Amz-SignedHeaders=host&x-id=GetObject)

