
[CH2] C++ 프로그래밍 기본  


> ### switch 조건문  
>   
> - 특정 값을 기반으로 조건을 분기할 때 사용  
>   
> - switch(표현식){  
> case 값1: 문장1;  
>               break;  
> case 값2: 문장2;  
>               break;  
> case 값3: 문장3;  
>               break;  
> }


	### switch 조건문

	- 특정 값을 기반으로 조건을 분기할 때 사용
	- switch(표현식){
	case 값1: 문장1;
	              break;
	case 값2: 문장2;
	              break;
	case 값3: 문장3;
	              break;
	}

### [프로그램 4-11] 주어진 날짜 요일 출력


	```c++
	// [program 4-11] , p.159
	#include<iostream>
	using namespace std;
	int main(){
	    int day;
	    cout << "Entere integer(0-6): ";
	    cin >> day;
	
	    switch(day){
	        case 0: cout <<"Sun"<<endl;
	            cout << "start of weekend" << endl;
	            break;
	        case 1: cout<<"Mon"<< endl;
	            break;
	        case 2: cout <<"Tue"<<endl;
	            break;
	        case 3: cout << "Wen"<<endl;
	            break;
	        case 4: cout << "Thu" << endl;
	            break;
	        case 5: cout <<"Fri" << endl;
	            break;
	        case 6: cout << "Sat" << endl;
	            cout << "end of weekend";
	            break;
	    }
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/de0f731a-da70-4761-8eb0-3e5c154e9b22/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466Y3GFQRCR%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044724Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIHwQB6AblHbS3pA3b6VckPBCfCWNhCsQJU3IPbt2tUtZAiEAjIuPr7Wkgn%2BhEAjSoGz8JSDUfxLUtfmJFk%2FKDreEAdgqiAQInf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDF%2BGyrCZqG7xkkv5bSrcAzsws0pyHIh3xqftyFT2kejcOzjP4qCpCoD8wJYgCBhG8AbH4lmKCGrs00cl81f3P%2FFWoQBWcKxKqukyEfNbsgs8oF0gKEkSuRbTlUleEep46n5r9Kzk0fyCLwpzcYV%2Fe0GpHZOG6SGERne%2BgTRO0Z%2F9uOFDbHdzOQP0Wna5J1GrEPF4qJfvVBAou9ycEkvrfhbeJ5bv%2BckPDBfV48vecE%2Buf3hxhOU9sBLYWyHxhUlcVO%2FMm49y7pO9ySNPmOvJQrKyA4oUsH0LgrgsV6nALBooQBhj4aMzuBZFomqhVP6oQn3NR77eeYLBBJHEEIuD8GteFHTTmBRdDNuXduQyAm7%2BAU0c2OjP89tsekQKXKChp0yjYG7bvaKL5ifueE9WEw%2B4jA80gE3oMT2NKKmZWrYWikFyG%2BP5RzGnob5a5CgSk0AgCZqDcRdWNdNFkODb3J7PztNpVvLEYm3udaClNjCPv6nkh6bpgols05VKqt3LY22Io2YDAV3LNT0gUY1wl%2Fr5EIMzdBpABOnkfWE0qtAAdWQQtAjLlBwM5HL5vuBhSPRNVIAPOeCohgCbOToKg2cQKIo0ZCw1wVa2GMwqEFK%2BxN5E0fMfGyGGBLORc%2FFIqYYTdDY7mTdwoys1MNbd5MEGOqUB1OImYRtbnQ7lc4uuZKnQU0td9kPwC26cvXc9JLUjOgzS1Mh7utUB0LOlapA8%2B%2BVeSaxzdwQDkffnKPhV0zmRLvhM1O%2B9qNVVT9%2F%2Bye5jR0PAVN38o%2FuS5LLvP8ulWcFDBdo1jgzGg1etvKfzElTfxi1NCWJ0sK3PxqNtAVNoAGIWWyNeFczO0IV2DhY9UPk45g7PtTyXrMTQrMM2YsKVlNISbhSn&X-Amz-Signature=9d5434371b273b72b57407dcbb2fdaa33bde29c78ce4824bfa7ba3e63822d31a&X-Amz-SignedHeaders=host&x-id=GetObject)


> ### default 분기  
>   
> - case 분기에 진입하지 못 한 경우 특정 문장을 실행하고 싶을 때  
>   
> - switch(표현식){  
> case 값1: 문장1;  
>               break;  
> case 값2: 문장2;  
>               break;  
> case 값3: 문장3;  
>               break;  
> default: 문장4;  
> }


	### default 분기

	- case 분기에 진입하지 못 한 경우 특정 문장을 실행하고 싶을 때
		- else의 역할
	- switch(표현식){
	case 값1: 문장1;
	              break;
	case 값2: 문장2;
	              break;
	case 값3: 문장3;
	              break;
	default: 문장4;
	}

### [프로그램 4-12] 점수 기반 학점 출력


	```c++
	// [program 4-12] , p.160
	#include<iostream>
	using namespace std;
	int main(){
	    int score;
	    char grade;
	    cout << "Enter the score(0-100): ";
	    cin >> score;
	    
	    switch(score/10){
	        case 10: grade = 'A';
	            break;
	        case 9 : grade = 'B';
	            break;
	        case 8: grade = 'C';
	            break;
	        case 7: grade = 'D';
	            break;
	        case 6: grade = 'E';
	            break;
	        default: grade = 'F';
	    }
	    cout << "Score: " << score << endl;
	    cout <<"Grade: " << grade << endl;
	    return 0; 
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/79356759-cfd4-4553-8674-70806b64ab09/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466W442JK7I%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044727Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIQCwjNitG6ixRtVNlPskN%2BVm6rBoL6QwCTONGy99m%2FyKIwIgSVP2Qapndsu37sxe1x4u3Cm2w66Eq1%2FfLExK9B3wnfoqiAQInf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDISm7QwXJzJ91Wxu0CrcA9mVVmM363DxP1vqksL490j%2BysuDCWzzr1uKqW%2BNugUvpYo5XI3mxYEcxy3ivDfqzCru9Iy7J%2B0cJvXTBuE7RAcagyKbYlJMKsU%2FfGDFzre4LvwUNY1JiJkbijb3DOrTxEltpb156HDBV5CsgeJJbNrcNsvqxrPWpxoEr39FTnDZCR1d3EepE5%2Bl5nX0LPkkxIJyOvEZWvpiGda5wQazTEf%2FVEQO7CGFoioZyZ%2F4OPLrl00ttpmv9dL403aC4g27Dx5LT6arWqsSX27%2FWOSmuVSGldp65zCub5STQ2ATfjZf%2F%2BV4EX0VlNfosKZmdOiz4nChtPysfmx4Cr0i5pB4Ndnm%2FNYe1LtrcQUjr57n4Op3DltYKG6d8oIdp2SC1yfzG%2FZXbBSzd%2Fvnu084NiLKOgglwzheXoFveCz%2FcJTVZbcfD5Kvza5UmG9Eq5OlI0PKNC3QZt%2B08c%2BPZEvEAbhOjILLzdcHLjl2an5HYkCLdRb4Oo3fZVhmLA%2F2TgCO%2Bsq13V7cCqssYHR91DaAjbEfDhhsFIgGHbSDbVO8qbG%2BwirBt%2BA5FeN%2Bo7isSA9EWQn9tdVETA%2FVqlx3ojcUuQ23icIrhD9d9xYLehXPw%2BjoJY3kFVCd0Ovwe%2BIeJbMrMIne5MEGOqUB02phfsErw8XQjUHJQGUV7UI62Jl5WBFp1HGg3t9Qb9DB2yppR5ZqjAzbSkIZ6tk30hG3OWxSP9el0iJ7WBEZRoO%2FbFu0DrzC4h1hmc5lXLf4td5OBA%2FEegGKsFhGXJOYSOLRavwMtpCCMCb78mEHEBbKlaEEEO7UATJu9OvwjEm2T6IeWo9aEB3%2FDcgHDUd57OMMM5uq7vtkMRUFDW7DNEGShYN%2B&X-Amz-Signature=85e200f92a1552fea597585738a5d116c8c3ff17b0d4bc9af408d3b919346699&X-Amz-SignedHeaders=host&x-id=GetObject)


> ### 분기 결합  
>   
> - 실행해야하는 작업 같을 경우 분기 결합 활용 가능


	### 분기 결합

	- 실행해야하는 작업 같을 경우 분기 결합 활용 가능
		- switch 조건문이 case 분기에 진입하면 b<u>reak만나기 전까지 모든 문장 실행</u>

### [프로그램 4-13] 학점 기반 Pass/Fail 출력


	```c++
	// [program 4-12] , p.162
	#include <iostream>
	using namespace std;
	int main(){
	    char grade;
	    cout << "Enter the Grade(A, B, C, D, E, F): " ;
	    cin >> grade;
	
	    switch(grade){
	        case 'A':
	        case 'B':
	        case 'C':
	            cout << "Pass" ;
	            break;
	        case 'D':
	        case 'E':
	        case 'F':
	            cout <<"Fail";
	            break;
	    }
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/bce8fef5-b280-4f1a-8ce0-a03fbbe5755a/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4666YRKLDH3%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044731Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIQCrszkATOL2%2BC%2BW%2F1RcmXFTW96kM7xRzSpb0jcB97aHlwIgL4bH2hlPTHu20aiA07aIS%2FqYVkp0PQChqDxe4VEzx9QqiAQInf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDNEwR%2BfqAUA7obvz3SrcA5%2F3QmgDMueqxqCjNt8CLzllFAfXfO1LUrXwlEVCw%2B18m7s7RrlLwWj3H%2FvHltmCF0BVMGQ2o7IId4Rj8Qj0nb7%2FSfNW2dt5C6uNwPv0F7DGJjTAfJYNYamDrxSd%2F7uxvkasnDFsH3QAsOihEYN7xC8bkrPVjX%2FkJBP0%2F6F0N3lNXhSqT6UHX8odkVSkFJEQGBmVOJoMutEKvS5iQtmnTaeqle0YxJxfT32w%2FTYKvlmuSU6xpi4fk3KgkuxFloCXAqYxjJxOm7tjrFUwlxyaM%2BEe8mOsdgfZTSkIIZK4A8uP1pRKQRsuPO2M7bHvrJ50oMXg1Izovr1F0tiYg6to9Lv9KZAJ49l92Vx8oDh0g%2BNY1Z1%2Bxlili3cs5oH2M7CIelhJnJi%2FXz16vfkMqNGDyYBUxoWVxxUoBv7XIca50oY5Ddxuz3mMR3jk5M%2Fh6KK7Bu69eo3JMTfSLUmI9KUhsRuF5Bk7yhRFyccwli3n0nx2%2Btpc%2Fpph9PTzjd%2FF3huysDOPSsjFU6hEa7WMZLSq3edWF7lJT%2FIDp10V9t6OUPboIFBnpdvD2MJNC7dcHdezptDyNy1BWbGWOYS9nJeXSLk5TyLGG6M3jip8vTLAgpTZRV2OP347d1cJng0aMKbe5MEGOqUBvVMwHTgnK%2BQ0b6zXAsNUJbKcCLTFHRylEBVuAbj9J%2BnBssGoXHQ5DSHqBMmenvuM8ktxmuIGmgm9fVYyR8U0ZueeUJA2U4j88f98NulCKLeH1GdR2Aihs%2BXWsMqeof0BjFSsRedRaI2wQ2nzVl0Fzzzvzo8uCnV74t1VvjcdzEAf0ikedcbGxB2zvPfAwd%2BDRMMHtLaeoqdJmxVuyBUaLvSu5nKP&X-Amz-Signature=e7594fa74e3563650d1ea1a31bdcc8adb7e658478286ac09b925159e8ca824bb&X-Amz-SignedHeaders=host&x-id=GetObject)

