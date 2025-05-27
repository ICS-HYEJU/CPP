
### 01 


	> 💡 `numeric_limits<자료형>`  
	> - 자료형의 값 범위를 알려주는 함수

		- 자료형의 값 범위를 알려주는 함수

	> 💡 변수 선언  
	> - <자료형> 변수명 = 값

		- <자료형> 변수명 = 값

	> 💡 `signed/unsigned`  
	> - signed: +/- 영역 모두 가짐  
	>   
	> - unsigned: +의 영역만 가짐

		- signed: +/- 영역 모두 가짐
			- +max(), -max()으로 범위 확인
		- unsigned: +의 영역만 가짐
			- max(), min()으로 범위 확인

	```c++
	#include<iostream>
	#include<limits>
	using namespace std;
	
	int main(){
	    // short -> signed(+/-)
	    short shortmax = numeric_limits<short>::max();
	    short shortmin = -numeric_limits<short>::max();
	    //unsigned int
	    unsigned int intmax = numeric_limits<unsigned int>::max();
	    unsigned int intmin = numeric_limits<unsigned int>::min();
	    
	    cout <<"max of short: " << shortmax << endl;
	    cout <<"min of short: " << shortmin << endl;
	    cout <<"max of intmax: " << intmax << endl;
	    cout <<"min of intmin: " << intmin << endl;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/3f2ee7ff-19cf-47f0-87b6-dbb3e5652811/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4663I4D6G3E%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074225Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIQDpYinOZKWhqFwMi%2F1KT1L%2BnI8HE7IsQfDAA%2F8lsct%2FjgIge78dL%2Ffn5qqD7AP%2Bhg%2FNFctnVvH3CiXpKezLHxoVuYwq%2FwMIVxAAGgw2Mzc0MjMxODM4MDUiDLSRJIKiM62AxZM%2BcyrcA3bsd0ssq8t%2B0XmlYKWtXDNXEBxfNiRSag7wWUNLlde%2B4BYZWAZ9L8pWAkig%2FMQ0kTIoZfG7IRGeHLLsBLHleT%2FEBHZQf%2BY%2FoKmMDYH5hhH8703p%2BMF97noQYCKR%2BK4dhFSLNfQmCFnVt4IfcWJbCD3HC%2BeibzmjSsKGIurTVngLDrcBUiq9kDtdXp91yMxejf3etafxeeq6cWWNuQepu4VM4h63cDDj37icTxkXWYGcs1hwmqKunR4GS9O47sWkBGeIL8LkwTyDE9JMITx%2FZXEemd9iEkhuG%2FoBBWu3Xz3SJMRfQ2HzLX6SEQGjfwzRwOZcUUjk04DX6C%2FUPuRqnB%2F%2F825QW4kzSb2Ec6PXzzCv7TCGBi5vpD%2B1G3sqanTkHvIxM8CkwxY2tYzljFTd1B78WVf2Yc0JhyaKYZ0nCSUXLrMUTu3wA5D0tzxG3IvXIpFnLA7Kq2UJL5McS4FhRY5V0CkGSdcvXzPlV38lzwGPw19beLyULlNzqODU7QoBP%2F8r8JlSruj%2B5i11BOSVEG0VZGMU9%2FdvMKHkQcWpQdccr5WMwkByPof7Eyyp4J3uXxyyzhTjpFk6dMl02Rw7JWCUzwXOImmmSzNp4R7PctgQF6CdPqYqSrw3NM8UMI601cEGOqUBn%2B%2BPAGY6eU1tLbfF%2BMfP7W%2Bu%2BKDZIRQtYYzx4ZriePaiZw1bJyrnThz9X%2FhLZb4YA2Mr6odTDfTBNU8Q6Fb77EkTb4D2TyA2TruHQ6VRuncGshH71ioJpJPk1Wh2XmMkJ5TrG7EGRY5CfOt3prodxWYfmwf7reNxRdng30PILz435oV9OxtEubB%2BiMpmddmGSL%2Bs9fKq2ISlAQHQGiIZ%2BBhRF9t1&X-Amz-Signature=78ad02414932a47363c1057936e8916e0bca46a000361b3bf5975695750d83bf&X-Amz-SignedHeaders=host&x-id=GetObject)


### 02 


	> 💡 long  
	> - 정수 자료형

		- 정수 자료형

	```c++
	#include<iostream>
	#include<limits>
	using namespace std;
	
	int main(){
	    long longmax = numeric_limits<long>::max();
	    long longmin = -numeric_limits<long>::max();
	    long long llmax= numeric_limits<long long>::max();
	    long long llmin= -numeric_limits<long long>::max();
	
	    cout << "max of longmax: " << longmax << endl;
	    cout << "min of longmin: " << longmin << endl;
	    cout << "max of long long max: " <<llmax << endl;
	    cout << "min of long long min: " << llmin << endl;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/0147bef0-36a8-4f15-8bf3-0555f2c50d09/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466RN622P57%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074240Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJIMEYCIQCHSKmeXXR%2BeTuydNrFWI5pivzKw71xsEdFxfBGscrBRgIhALdrnwGc8QQdrEDmgwgICfl80lWDYC3heHQV3kh5A3xVKv8DCFgQABoMNjM3NDIzMTgzODA1IgyvNqf%2BEMpht6o0%2FuYq3APMaikZ4%2FjRpi%2Fzz7gVSTXtcrS3YkYqTCW7z%2B2ek%2FQDm5WNg70jnMp5EQZ%2BCU0tyVsK%2BfrcIPFqEtjYn8AywcumOH16ZotcO6wNbvLDHSc5WFGhkaOFK%2BI2py114Atyx8mQyFWwHizcJjKP5KSEmQi5kSE1R6J2W0qzfv31XqjBN0igTa4VKB4v9Mzh6av0n73zi%2BljcwSXeoa6wJtvjjlNE%2BjGYUpaLB1SWBidVnVDY7Bsz2M3fzcnN4uGUIQjYJCFGUFHuLI28VdSoJJMSTFDGtualGpxG%2FPW47u%2B1IplJMG7WWDZYvaHo8uvb6QvgZWQ02GnJaPWgnhlFFjlrbYQbrc%2BDQuxd%2F0TpxTR0QQUHmHJVHxkyD6k5ub2X7fzbsOC0j5W2kSublQjAhc9HGnH235gvXPjbzmMLyVh9L0r0JhBYF9cyxAPWe7z9VrWi6cqhjSrgitm5%2FCvNfVu2CT7o51FHLZO7By5WpivuDmRbuIO9lBq2vXwXtXorsjv80l3TeZQDzetkoE4RktE8PXtbyWLnXKBqs1lNdfaUTL6H8tpIirM%2FqMPTmoyX46k8G%2FeWsN7volEVUT9ixiBhDcKGg5u4n7uZNuFX2TA6yFDgfgpEacBKNGvGMDV5jC7tdXBBjqkAU2PFFiJ4K8hhs%2BxbV%2B5c6Oi1PaU%2BP0ed4andnuRKRAo7r4qed3FnxxexhCaRp9SD7IQb5suSKHU%2B7K6Fkwy37Dx6Rw4LG5mVDdIeVAfgRSag68e7t9%2F5U89RKBg4eji4wFHCWC3EIIE8JvY4EgbrfEjL11pCVqvUaw6QvEL1HAim2fmm2CNFl9Bbt3Z5Sx6Gqw584sKnl1RAU037gvp4rYn54il&X-Amz-Signature=50492e6f78efac2e5d8620ea799ff770c5651857f804e2f4871283ecd66f1820&X-Amz-SignedHeaders=host&x-id=GetObject)


### 03 


	> 💡 float  
	> - 부동소수점 → 양의 영역에서 범위 가짐

		- 부동소수점 → 양의 영역에서 범위 가짐

	```c++
	#include<iostream>
	#include<limits>
	using namespace std;
	
	int main(){
	    float Mf = numeric_limits<float>::max();
	    float mf = numeric_limits<float>::min();
	    double Md = numeric_limits<double>::max();
	    double md = numeric_limits<double>::min();
	    
	    cout << "max of float: " << Mf << endl;
	    cout << "min of float: " << mf << endl;
	    cout << "max of double: " << Md << endl;
	    cout << "min of double: " << md << endl;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/4b4b7c61-82bb-4d0e-830e-4fd8d541cec3/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4666AI5VIVU%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074244Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIQChYFmWvbb5dfI8%2Fkm8EOuAAwNQt%2FDGtL4CVD0Lb3ZKAQIgLt6ys0Of08UYyho7oovdOLJsn4%2FAFZqaF7zoDeyJraoq%2FwMIVxAAGgw2Mzc0MjMxODM4MDUiDPCeq9KmSGOluvDxKSrcA%2FRzjW34fNV8zJUc9GNC7gu4RIqW2CVAzbvz8mea1MXwFLORf2TwHbBkcBOalOuorc5Tti2EQwRJxsoANwtWyN1wVX12oFLJ2POyFHAxoj8i%2FLm56KdeCpJOdfFIUcAGc8kOcJclpS%2Br8JC06ahJ7iBGtkd7QfojJSgQcL%2FEvwzO7OKmrXaQiqF%2FKKvV83aG5xVyOjAj3gNGtDs7OhEGujKzztvXxvtFa6sSEtbPVz5XpmjShU1qK6SqHFmtpCQxDE5WsMy5TdI7GzVIGc3gTfdUIzdlXszbDvPzgolvSeSqyKoZKl%2Ff5rYRxu5wjaE%2FU7lrU45XNAl43o4GNrlEkm3f02Mv%2FMWUYFbfA1KBf04pPmsbWIg3vf5tEy3UsbDWuv4UR%2FPS%2BR10i35C7couH1K4kvzmXkUolcS2efE%2F29qPVoxGhiKZtiht%2B%2Btfvh0bak8r6807%2BN4JS%2BGzgW%2FRewbSvuEwLyUiIBGEw0oJKGMCbda5tOFd6QCtiBXC9C9ottCFCepbpO%2F4BAOHZqxgSoYLkdc4ELCy4tlaGRnLWuvrOGjufN1no0BhMahA%2BgY%2FGsmWcQM4PFs4fuXHXkvvJAxCrg4lQcrXHSE%2Fh1bmFVlcyl%2BkXMkJJqFzBX2tMIe11cEGOqUBBEBvfhuTHQM9SVVt5E%2FlQAwJpaOHEUkGy4rKcoYklBJQh2%2BeQx%2Bp%2BlL55m4ZaKcRQWUby5taYrfa8tJfojNhhvcZpt75x4CWr3tyQ%2Fz1VCbdvYfDxJTme45u3VzPH7P%2FZ28oPf0ex6AhwhPUsFR%2BhJP7cSnzyrhcavSsNx4IESsN7GzKREAAjW6qQZ6YhqN7nxykUPXfRkrLnbYKQRqkU4B4fDqA&X-Amz-Signature=c21476191310d0f266a93b1a30bf30a57e8af061fa725346d76edd6a03838605&X-Amz-SignedHeaders=host&x-id=GetObject)


### 04 


	> 💡 `std::to_string(변수명)`  
	> - <정수, 부동소숫점 자료형> → <`string`> 변환 함수  
	>   
	> - `static_cast<T>(value)` 사용 x 이유:

		- <정수, 부동소숫점 자료형> → <`string`> 변환 함수
		- `static_cast<T>(value)` 사용 x 이유:
			- 값의 구조나 의미가 크게 손상되지 않으면서 바꿔도 자연스러운 경우
				- int → float
				- char → int

	```c++
	//문제의 자리수가 십의 자리일 경우
	//12345 -> 4
	#include<iostream>
	using namespace std;
	
	int main(){
	    int num;
	    cin >> num;
	    cout << (num%100)/10 << endl; 
	    return 0;
	}
	//문제의 자리수가 숫자의 두번째 값일 경우
	//12345 -> 2
	#include<iostream>
	#include<typeinfo>
	#include<string>
	using namespace std;
	
	int main(){
	    int num;
	    cin >> num;
	    string strnum = std::to_string(num);
	    cout << "Type of strnum: " << typeid(strnum).name() << endl;
	    cout << "The second num is: " << strnum[1] << endl;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/c823f4c1-c26d-486d-9d33-86014921444d/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4666QMNS55F%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074246Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJIMEYCIQD%2Fg78xDfCYRdKoghgX1dVZ1Lj1TMd6Pn3DHMWiWofjNQIhAJ7H6v10IK5x4U8W5takRx7kIPwiEWUBUxfQtRf1c3klKv8DCFcQABoMNjM3NDIzMTgzODA1IgytdARaa1JV3VXEpxUq3AMcr2gOaB8U7uiLmjAy8yRCWrxyTcWB69Sq8kxvyX2HRe4PWT9NmSqTfIuez2bszVamscmxEVLavrX%2FgXH4B%2F%2B%2FXgqLZ5LDgAeUIPaWkfTQvOLaBUbi4m5v1Y049DrEg5UJj8aYEfhM0bBqST7rSKt7lz1%2BjbNe4%2FTLdWELg0KcKagPpEOCJiYTukiswdxNFpnLYPOZxVqWf0D%2BkhQymrYbuo9tfOQgF1I%2FwMld70qXWZMtULX3eip2KjjeMoHU2gbFheEst8HicBMOvcthfq0TA%2FUt2wBtFHcVufERRiNS2xy417%2BT%2BgeMntCM9Rbo6uBYaKrl8847wIUa1Bf8r8BkXbYjCgzbVbMlJEOFhEbKOe6gnJ%2FH%2BuZ99XKKtcrw6urOc02f0gFgl0bpS%2Bf%2FFgUUGvHWxXAAoZYrSh0vVyjZ9ps70IfdcAsKEbTTsEADSDnuZoAtsebyiovsd4z13dO90cHdqrkuNrV0gTG%2F2j7vW%2FoBxsk20Yvc3TFbbXGsLMKeuDwD3loGFsZuH2YCYscQmwcq9CcuDS60cjEWGQfQjP8FMslannHGXrQhR8iSQyFH%2BMJNNfjW5S4y%2F8Fu3eEG50OTKh1QHhIaLTUgtgUUIOCbDd3TeKmjNaUbOjCotdXBBjqkATTsfbEz1m0ZZOOoQmo7hWsRRDDMRvId8pzENEzR1lP%2FwVZWNHxOQ6q9WSd9oY8UQWrPfTTsi3OM7Tc6tEy4tq%2FgrfLTYOu%2F7e1g8YKrKsqeXRKaMSfA1lM8NuLUI8EMdaU1cSrGWCs0%2F3uBzmXM7kamCSwj0C8w7bAPXd%2BPb3p4kxab4AdbgY2eIrLjypThXFRORlXC6afHsv%2B3hyCdIMMfxyCM&X-Amz-Signature=c047818e8d5ab2ba10b87e4c5b11f61763efeaec039898ee047d6f0618e87757&X-Amz-SignedHeaders=host&x-id=GetObject)


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/0bc56074-e87f-4207-860d-e8d04b294f45/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4666QMNS55F%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074246Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJIMEYCIQD%2Fg78xDfCYRdKoghgX1dVZ1Lj1TMd6Pn3DHMWiWofjNQIhAJ7H6v10IK5x4U8W5takRx7kIPwiEWUBUxfQtRf1c3klKv8DCFcQABoMNjM3NDIzMTgzODA1IgytdARaa1JV3VXEpxUq3AMcr2gOaB8U7uiLmjAy8yRCWrxyTcWB69Sq8kxvyX2HRe4PWT9NmSqTfIuez2bszVamscmxEVLavrX%2FgXH4B%2F%2B%2FXgqLZ5LDgAeUIPaWkfTQvOLaBUbi4m5v1Y049DrEg5UJj8aYEfhM0bBqST7rSKt7lz1%2BjbNe4%2FTLdWELg0KcKagPpEOCJiYTukiswdxNFpnLYPOZxVqWf0D%2BkhQymrYbuo9tfOQgF1I%2FwMld70qXWZMtULX3eip2KjjeMoHU2gbFheEst8HicBMOvcthfq0TA%2FUt2wBtFHcVufERRiNS2xy417%2BT%2BgeMntCM9Rbo6uBYaKrl8847wIUa1Bf8r8BkXbYjCgzbVbMlJEOFhEbKOe6gnJ%2FH%2BuZ99XKKtcrw6urOc02f0gFgl0bpS%2Bf%2FFgUUGvHWxXAAoZYrSh0vVyjZ9ps70IfdcAsKEbTTsEADSDnuZoAtsebyiovsd4z13dO90cHdqrkuNrV0gTG%2F2j7vW%2FoBxsk20Yvc3TFbbXGsLMKeuDwD3loGFsZuH2YCYscQmwcq9CcuDS60cjEWGQfQjP8FMslannHGXrQhR8iSQyFH%2BMJNNfjW5S4y%2F8Fu3eEG50OTKh1QHhIaLTUgtgUUIOCbDd3TeKmjNaUbOjCotdXBBjqkATTsfbEz1m0ZZOOoQmo7hWsRRDDMRvId8pzENEzR1lP%2FwVZWNHxOQ6q9WSd9oY8UQWrPfTTsi3OM7Tc6tEy4tq%2FgrfLTYOu%2F7e1g8YKrKsqeXRKaMSfA1lM8NuLUI8EMdaU1cSrGWCs0%2F3uBzmXM7kamCSwj0C8w7bAPXd%2BPb3p4kxab4AdbgY2eIrLjypThXFRORlXC6afHsv%2B3hyCdIMMfxyCM&X-Amz-Signature=ce0c52bd493b46049948d7480c6cee2aa80cae3f03f7c4d18fd2a1e6950500a4&X-Amz-SignedHeaders=host&x-id=GetObject)


### 05 


	```c++
	//왼쪽부터 자리수를 세는 방식
	//왼쪽에서 n번째 숫자
	#include<iostream>
	#include<string>
	using namespace std;
	int main(){
	    int num;
	    cin >> num; 
	    string strnum=std::to_string(num);
	    cout << strnum[0] << " " << strnum[1] << " "  << strnum[2] << endl; 
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/170b369f-282a-44f9-8c9e-ef38fc1af838/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4665JCAFNKK%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074255Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJGMEQCID0CI65dizD7bFYvzSXJsm7bxMJAgVHVOL24gzNKJX%2BZAiBUF8PxgBhdLpLIJLNLNm%2FtxhkiDe1mQx4ccxAz%2F6UGpSr%2FAwhXEAAaDDYzNzQyMzE4MzgwNSIMwdqoYxoI%2FigskcDZKtwD7%2B58H5lVdg%2BVkmccvq3A8nvpXDn%2Bjeuj6oQoAe6loy6ISvEYDDokuqsnBQrQ9TUULdlu9sBvVnSfRFA0%2BS8N0OxLMjtBtpB99thGFWe2EwLFZ%2BvVMj0rut99UmRjfnp98p%2BMoGhkEoC%2Fx5twsw5Msx7rpp7Xq3NjbdOc4IlGWjU1Lj%2BwL9KwVRbIQ5QMBa%2Fv19rNXUHPRyJvA%2FCZ4qKAm%2BR%2FjnoVJKW7S5yDFZTtFFJr8rpxS8qNsyOV4tIl8sYZNjWBfDFNwRB8mV4PXsoTcNzskHTk%2BrGnI7oZ%2FUXyt4UeL%2B0QzJDWBfR6%2FLqdTcPX%2Buwc723ZHxPthwxbR%2FA%2B4EVhuEddXAbUE%2FAXKqqHl97DgDeUIcHONa2GEW1gdDrqi3MRS%2BDD8yy1YxXiEvwFjkwLypcCSF5xshYN1d9hRyw7AEfcdW%2BEK%2F2hlYoH1%2FNl1UNQoRI%2F5TW0sVkzchpwJ7iYEX4qSwT18BhlwfXXNQ3Na%2Ff7aTknJTSeiH8GBjAE7OckebZTUINlU6OIgLLsvX93aWDTyR2HXFdQoAuw8k7E3AFGxiFi%2FBGIx1QcuY3jPQu7jQWE0IW%2BTVvgXo6tjMMgXMJFBrA4zCy3MYt0GSEDbGr0PATM%2FGd2vxEw6LXVwQY6pgFZdB4EAh%2Bmyee8P5rOJ5%2BaPUJtISajc6w6YpmvopEWXoI5asraHdHQbt5Ctibq2AF4Z9ZeqpUw22zPHGyl8RCgLA4w%2Bugg9gvvSvLy621OWWxwhlxQm7B3f2fi5lwYOc6zckcdwhzt1%2Fq0YvEUtOGfna2HN1VaAq5dSVYsiVVwLcX3xxGt0%2FrVpG%2FMyCo5ls%2Fiz5e8R6GI4U%2FUGmJpPdkxBWyf12bt&X-Amz-Signature=b05b50bbff358310aa5dba124586389214b9ca9dbdd21b8e23cb48ea6e06d198&X-Amz-SignedHeaders=host&x-id=GetObject)


	```c++
	// 오른쪽 부터 세는 방식(자릿값 기준: 일의자리부터)
	#include<iostream>
	using namespace std;
	
	int main(){
	    int num;
	    cin >> num;
	    cout << num%10 << " " << (num%100)/10 << " "<< (num%1000)/100 << endl;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/3ccf5f69-9d74-4882-8116-6391ce387172/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4665JCAFNKK%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074255Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJGMEQCID0CI65dizD7bFYvzSXJsm7bxMJAgVHVOL24gzNKJX%2BZAiBUF8PxgBhdLpLIJLNLNm%2FtxhkiDe1mQx4ccxAz%2F6UGpSr%2FAwhXEAAaDDYzNzQyMzE4MzgwNSIMwdqoYxoI%2FigskcDZKtwD7%2B58H5lVdg%2BVkmccvq3A8nvpXDn%2Bjeuj6oQoAe6loy6ISvEYDDokuqsnBQrQ9TUULdlu9sBvVnSfRFA0%2BS8N0OxLMjtBtpB99thGFWe2EwLFZ%2BvVMj0rut99UmRjfnp98p%2BMoGhkEoC%2Fx5twsw5Msx7rpp7Xq3NjbdOc4IlGWjU1Lj%2BwL9KwVRbIQ5QMBa%2Fv19rNXUHPRyJvA%2FCZ4qKAm%2BR%2FjnoVJKW7S5yDFZTtFFJr8rpxS8qNsyOV4tIl8sYZNjWBfDFNwRB8mV4PXsoTcNzskHTk%2BrGnI7oZ%2FUXyt4UeL%2B0QzJDWBfR6%2FLqdTcPX%2Buwc723ZHxPthwxbR%2FA%2B4EVhuEddXAbUE%2FAXKqqHl97DgDeUIcHONa2GEW1gdDrqi3MRS%2BDD8yy1YxXiEvwFjkwLypcCSF5xshYN1d9hRyw7AEfcdW%2BEK%2F2hlYoH1%2FNl1UNQoRI%2F5TW0sVkzchpwJ7iYEX4qSwT18BhlwfXXNQ3Na%2Ff7aTknJTSeiH8GBjAE7OckebZTUINlU6OIgLLsvX93aWDTyR2HXFdQoAuw8k7E3AFGxiFi%2FBGIx1QcuY3jPQu7jQWE0IW%2BTVvgXo6tjMMgXMJFBrA4zCy3MYt0GSEDbGr0PATM%2FGd2vxEw6LXVwQY6pgFZdB4EAh%2Bmyee8P5rOJ5%2BaPUJtISajc6w6YpmvopEWXoI5asraHdHQbt5Ctibq2AF4Z9ZeqpUw22zPHGyl8RCgLA4w%2Bugg9gvvSvLy621OWWxwhlxQm7B3f2fi5lwYOc6zckcdwhzt1%2Fq0YvEUtOGfna2HN1VaAq5dSVYsiVVwLcX3xxGt0%2FrVpG%2FMyCo5ls%2Fiz5e8R6GI4U%2FUGmJpPdkxBWyf12bt&X-Amz-Signature=56c0b727f9aacdf22108d7a22336265e3c9fb6483c6686030c2606eb87a272be&X-Amz-SignedHeaders=host&x-id=GetObject)


### 06 


	```c++
	#include<iostream>
	using namespace std;
	int main(){
	    int num;
	    cout << "three-digit number: ";
	    cin >> num;
	    int invNum1 = num/100;
	    int invNum2 = (num%100)/10;
	    int invNum3 =num%10;
	    cout <<invNum3<<invNum2<<invNum1<<endl;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/a6fb6ccc-b595-431d-985b-cd6634fb2791/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466TCQLPLRG%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074256Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIQD3Y8o16Nh4fJLsBlHnhGCK3xwHwEVAFxi2LsAfP6boJAIgaOuNDlQ9JyjMwxc4c%2F%2Bxklz3UQfzyg6zVPR4kc%2B3pMAq%2FwMIWBAAGgw2Mzc0MjMxODM4MDUiDFvgYbC7ynGtYOgC0yrcAyuW0T%2BPl8Tvc6N9oo9sNwviSxanp2ZluYNp4Za8Nd3r1Fj9tsN6%2FBJ%2F26EACCOF4K73U5tHt9MXGdtiJTpuUYgxrR6liC25iZkhvkEhdiWi1RWPYPSwIT3f%2FmOeUU3yH62E1eydR1t%2BVTHITtPpwEd%2Bff8Npbal19ISaX7HACOCWto0xiCBStsUeHDulNLvKcp0IypTF8YyaUehTNEgm6xpf8KUOaIMnnGRJQ12RJ74Duetk3KvPI8tnhHT0H8yGwz7FdcVCnDwoPz3eVxfkiyqmmroERrLxyQ6JjU6pDOdPmdg1YHzJXBSdiwT9iA3CXxiMYyBUjWjJZsnvfAACNFYQE3NKSKKxFhGm%2FIYkCJBvA3%2BZFeCLE7mtuJvWnLEM%2By4I5zQcjx6FtPcVPhCHlKWxkEwVku41BnJVkcOUKbWTm6zzYSgTLx9metK%2BiTloHQfpgYb5q9x1ruqvGGqspDyM2tlfsDCfG8T1m6B5hUkk%2BdDUD0G1E%2B81Bs%2BxoBR6ZmSNlJdXoaua1O0e1v%2F1dDuhYs6UGYVg2RE%2BNuOCxHDxwBP39Q0WRChSOF7IrkNFf0S5aLA7pOw%2Fb3gG%2FiLTUL7BH5Dwa7fElN5X05mwWws1gCS1SBb3VyrD7mhMJO11cEGOqUBMyy223lxfDfQ6csYevgIxJ8YiUTiQqqxtWWlWnpD6cYkm3sNzAJOMCxterZj2ZMgJ0o%2BE2FK%2FwcdwvAE6WMFi6WLHdHyQ6sEHTWZ%2Fc6AMrOrOSB%2F8IkyaROoLCc2gNLWNn0HVCu%2FzYmM7IDdSi2s59N9SbmnU131KqQm%2B04pXEaPBRhIiCHNzZCJyIaf8boYFJdnAIZpbdJQej4qmK6cC8DicHtb&X-Amz-Signature=b4e33873bdf6619fff3efef3866a1091bc8337e754c34e16ed9abba2be08133d&X-Amz-SignedHeaders=host&x-id=GetObject)


### 07


	> 💡 계산문제 검증  
	> - 알고리즘 확인위해 검증하는 코드 작성할 것  
	>   
	> - input 값과 알고리즘대로 계산한 값의 결과가 동일한지 파악

		- 알고리즘 확인위해 검증하는 코드 작성할 것
		- input 값과 알고리즘대로 계산한 값의 결과가 동일한지 파악

	```c++
	#include<iostream>
	using namespace std;
	int main(){
	    int totalHours;
	    cin >> totalHours;
	    int weeks = totalHours / (7 * 24);
	    int days = (totalHours % (7 * 24)) / 24;
	    int hours = totalHours % 24;
	    cout << weeks <<"weeks " << days << "days " << hours << "hours." << endl;
	    cout << "check: " << weeks*7*24 + days*24 +  hours << endl;
	   return 0;
	 }
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/a6fb6ccc-b595-431d-985b-cd6634fb2791/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4665EYYQSVW%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074257Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJIMEYCIQDwwHlkt75VsoffchYHnXEFpjKpTPi4Wga04TR9NNAmMwIhANfTlKw8ryUagICwEivIdudVDmn7EdXuozaRb5eSn0ffKv8DCFcQABoMNjM3NDIzMTgzODA1IgyeiBvMN1sGkLvrDIIq3AOCP4qfi2N7%2BCm2JiIBAhbbyVo4l73wOAyBaEKPZGo%2BIBjEPVzsAJ1xuAYs0Xr85gcUDFWdh3dnWTeB38dgFceRV3Lbl7%2Bc2rbZxcr2PY3SOZq8H5%2B2gx2mLmXNGtp1yDLZJ1V%2BHae1uhEI7uwBpXD8HK1MNG3NpTK55iBpdP7a3i4flhlsNX0lT0HVXDIMauc2qt8r7kw8d4r8PNzIC6Su92Vr9RKbCjwpCzKNBiW0cy4hK%2B%2BosAXiFpsH%2B7bHRJpd93cAf%2FOHzq8aptNhODZBHShveN%2B1uKhxXKL41xEhqaV0hkunBDdxPIVNWwe%2FxyB8kBA9iBS5IOC2uqXQTcALFuFi4sPioGXTImmVg5XQFk15GEnmCvlPqTDi7dfnsi6BqiEyPrBY7e9B8B%2B5%2FX9jzl06mio4YCcikd3DmbHNJbK48TXbtf6FRlbhcGUoXpHlu1nururLGH8UcbeMXRntWKibJ43UKCK6R1b8ZxS0UzHqvXjT0pYiG29GSTUgsrb%2Bs069PEDc7fK7fJZATdKQ%2FbzI7ncR9qJoYae1xufB%2FdmaWALIG%2B0Ax4kZ82H%2F9TICQ0mRcNUmZ4xOT0gLgkGjrrInFx2J8sDgV3K%2F0iIgTEuA%2BAJWpK3W7a6AKDCTtNXBBjqkAR%2BOJgGbR5SRJiJ3Sf9Ik4mFJzKEGQNNEE6KNY53RaAv5oU6Cx4oUx1%2BnJVE5PZ%2Fj8CATkW0IK%2BkBd3ydHZfpf38N%2FTXyp0VE9EFk3X3U1JXxLaW3DjZEpHBy4mP7bcE2bhSW3emPAAwM8DD7GPT3r8NjNEJ9cPLHF9exaHapNGDRokDzstj2qvl%2Fg7CWPk22dSYBqkYQweMVzkrzkkrmBCprRf8&X-Amz-Signature=01d71b0e5ed69585e3fa5dca0138aaa1db41ce070d1552511f4427990f74ec91&X-Amz-SignedHeaders=host&x-id=GetObject)


### 08


	```c++
	#include<iostream>
	using namespace std;
	int main(){
	    int hour;
	    int min;
	    int sec;
	    cout << "hour?: ";
	    cin >> hour;
	    cout << "min?: ";
	    cin >> min;
	    cout << "sec?: ";
	    cin >> sec;
	    int totalSec = hour*60*60 + min*60 + sec;
	    cout << "totalSec: " << totalSec << endl;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/f873bc95-d02a-4233-9ac8-0a9e76a3d07c/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466RIQDHNP5%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074300Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIDE7dUNuEPzXqTLyXRvy%2B93wQQOUagTZbLEBfkwTZrJvAiEAxqfUdlDsAQyCHP4I9ClUYdv2pZvb3rMMji%2FOqaZL5woq%2FwMIWBAAGgw2Mzc0MjMxODM4MDUiDKGOKYXUf555D5vy9CrcA%2F7%2Buzj5%2FqjN3P7aUugA4E1OoE6W%2FOgUo%2BsFS2HkVtSr284aYo2gTm%2BlBn%2FL6nhVOz1C2u9FLzZ4HsoQ9%2Fl7FzZdrQ4yjT5HN%2Blm6ls%2FedbGgFqylKeI%2FmfmlGO%2BS%2B%2FyCWuEOzz5bQpenKtSH4a5j%2FQEDZSvSQpvcqJFdjGR1si8yzCTY%2FfHRJiouHhJOm01eMPiac9xsT1SscktEq5HotjIpyqMoWNUy9h73LWJkh44zGbLmfXqdjn1hOOHYPI8cyOBBrvGG%2BE%2Ff5x7fAUSRTrckF6%2FpxhCNEwAaDumWbNsLj7LH2VzlGHcpeLP1GXLtDyScmlzSX%2FQXFcIU9d5Ab84IO66fLUj7eUrzolX9RiIX9QVMm0tJZ6dsM%2FQUqTLMhA0oMQIJb7UDt2AvPIa8GeTmk%2FHdAz%2BOzwd5kZAPX4kCp3JJKrq26LlsG0N%2F8e0XjRygHGyN3%2BjguTVyg5u5W9%2FhfNj5m8ePoQ3ObKqam64ZQdiHQwjjztItJithvWqTIdwxpzF8D1CpZgjxRTHl57kpoGLZYzTqm2mUrtqkKmApkotMDK1gCRkhGkggU8uIzMjhFgXQucpg20BJEoaYOsv4%2Fs%2FUKW07RxUq8cM7ziSsS0wgxyDhlAiMjhNMOS01cEGOqUBnYtqEzqwRof21HjOusbLshnVFHkFeSt5ho29vW2XbJ1hplR1u791z6HD4Z63SSmZu9xcLEAnglvQItqYNgwlH%2FnqzWI7WorNMrBfmGemHyxkJnFed2xmXwi3OD1JxhtOeTryAt7nmC5GMcTtyWUaeZPD72uzlhgjNFx4KhtAD8IDgJtlKEvUNkx%2FwDJmNJSHwV28w8IQtPwhawE8dTejC4nF00U2&X-Amz-Signature=ea366c65693eaf320433599e63fba0a37b6af180b78f772ed82543f472e0469e&X-Amz-SignedHeaders=host&x-id=GetObject)


### 09


	> 💡 시간문제 알고리즘(주/일/시간/분/초)  
	> 1. 가장 큰 단위부터 구하여 값 변환  
	>   
	> 2. 각 단위 계산시, **상위 단위의 값을 제외**한 **나머지 값 사용**해야함

		1. 가장 큰 단위부터 구하여 값 변환
			1. 시→분→초
			2. 주→일→시간
		2. 각 단위 계산시, **상위 단위의 값을 제외**한 **나머지 값 사용**해야함
			1. (totalSec%3600) / 60
			2. (totalHours % (7 * 24)) / 24

	```c++
	#include<iostream>
	using namespace std;
	int main(){
	    long totalSec;
	    cin >> totalSec;
	    int hour = totalSec/3600;
	    int min = (totalSec%3600)/60;
	    int sec = (totalSec%60);
	    cout << hour <<"hours "<<min<<"mins "<<sec<<"secs."<< endl;
	    cout << "check: " << hour*60*60+min*60+sec;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/27f41a57-4f7f-479c-b320-f0f586cdb0e0/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466SJ7MZNIY%2F20250527%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250527T074301Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEI%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIEXVlGUGYf8hUoiR006lutMvsJ%2FAHcjSwgWaSHvLgvETAiEAo%2BGxVjSXn95kksdSAjPosC60YfWNLHoXTXpNpgxOu6kq%2FwMIVxAAGgw2Mzc0MjMxODM4MDUiDPkqM4pskp9CKHTJXSrcA9zMrueGYvgm2%2B7yeqMUmFrqRrg36dnjpY3Bu%2FBfC%2BoCKf6BG7xj4Ro%2BPg26MHgicvMCFIHGxlibb6kVYpQnM%2FOxK5Y9Rhcm1NOybhCfxv6etLZR0MKSFB2xupLWgthiP6RLdozDxsqHcGHQi3QFWmtASmoi5zwRxy13y%2Fksxflg5ARxwfplFL2tiYwtk64zt01bV5ZObIIS7OTSqHV23W%2Br3OSz%2FiEnQBgLBxzb0%2BXaJvSpX%2BRpyKLWdUt%2B%2F6qAv%2BFzdumkObxNaJw4iWRw2AnXpuhBxmw3rd1JiomAVwHwhTvekxKofUiFQT6o6ocFQ3%2Fb3vyf91F%2B4a0C4umvn8alSU0WDs2K1peOELh51kFpxMcCbJAkktZVw1u%2FGbvyDo%2F9FnzqlYc%2Bht%2Fx5YxTJzYRY036cLwjHOMNeZMGA5BVmZg1qUXAm%2FshRjQzMZtWFx1kairszAUlw0doQE1cehigQEWRHTIp6sFxOwVbTd0IjvCyYt7iIGCMEFhyp1o8UsA87RGuLqhw%2B9mEhmYjR%2BHOcIn%2B2Cadd%2FJaUEy5ejTXHHxljaUwZyfo%2FSLmJ67Q%2FRJDFzD7G1CQljybCDfUfaeuIbqKn%2FRrgW8ip4%2B0gyPiYmPD3QadUJn4yELxMI601cEGOqUBiMyOpqAv0oJgTRm7McOkWgGOokWNOsTSFKvIn3%2B%2FVE9SjMLtIrGl9M38OS3Ky1P0Zj1%2FrAZT1988GYi6iLg8dqWfsG5ndJSyW7LQEPpuZrs2YbRhydoQ%2FneOUIV5JipO5CYen49CL24%2Brs%2FVnvunqw475%2Farny5lywu8Jjvt4a3dV6ghna%2BspF%2BU8NfaIjHDreTiz9AWJywjGQuBV2yP2vzq4Ik5&X-Amz-Signature=b2fba52036f528dd06faf1e6b38ecb30c6201bd2552649f3e56061508ea5b03b&X-Amz-SignedHeaders=host&x-id=GetObject)

