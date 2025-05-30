
### 01 


	```c++
	#include <iostream>
	using namespace std;
	int main(){
	unsigned int num;
	cout <<"Enter unsigned num(2digit): " ;
	cin >> num;
	unsigned int one,two;
	one = num/10;
	two = num%10;
	cout << "Result: " << two << one << endl;
	return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/1f465778-3db7-44b4-8f48-3d2c330d772e/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4662D6HGD5K%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044756Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJIMEYCIQDMNvBCpA0bGm330Yv6kiHny7L2rdR%2FGx36WvrOzlD8oAIhAMf1r9ym7NUla1VrRdhvKIk2B42j3X1FuP%2BAji57JVOoKogECJ3%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEQABoMNjM3NDIzMTgzODA1IgzjRaUhP%2BLT13yma%2FUq3AMsJ9qT68oQQxs3PKy9E0qASXQUEgvMYUpvR8eoPe6vkwG5SdQfx%2FNYV2Mt6%2FBrjpbwupdMFX3M5H7kDOUfpQJq%2F1hNf54W%2BpqAQifBS8bSMnVeLiS5sQtGlLCUfs%2BdeWiUXGPQURz%2FAxEVvABcwfzIdxVCLTcA0AVFPWNcH7YBMevvN%2BvJrcqzoGRN6x1wRLzRoJTeRumxr1g8M2PXr1KCIwW59WWoqSxn90HReKAFb6eE3%2BDkLLAFS5mpnFWCd8f9D9XjmCYRFC89WahBTogbhui9M8L%2BPxBr96JHYNhFrjypHOGE0xTrnb0gAAdteDZnfJBOZ%2BwavmqqPRhl0dSwvcerS%2FRKx6MkJCedyLGsaKghLwoqQSEMwHAAV2XmiKWyRs0ls0zWzSeK3SIZisgIPPetvDuP0aj0I8pGMBS3YpBVCi2yPYm664h%2Fw44krVELN%2BP9lmkQYzyM1J76hvAbpEO%2FYbKOYCPkHG73jCNYbmibTD226DK1357LBzR0nLDrIOCGc1NPl90rC53Mh%2FtgSLvq6cHYd0lS%2FXA1PXwFKgddWShOEh5Ytdr%2BuTwNEup%2Fu2xEeumwae5ZGyjLGxbufznP9ywcCMlqFqo3sb9eHbBbUYvJvanC4AjRQzDW3eTBBjqkATTGjN4rxsuipMMGgmUvD8lK2LAwuy6WStA1pcUMTeOAhJepN6nH6%2FjJpBeg5kVBbY37EM%2Fu9v7N%2B4Ct1Lwz7xC6pLGs7tmYHS0d60MUp%2Fl8pgj2hIp%2Fn8Cn%2FkHXPNokNdnyPlMZnxBljlfmasCeYd%2ByWTwLI44TsIT3US9%2FgpdtFA5BGHfpXIJ3FtVILLHWDVjSjGnax8kWr%2F4R20G%2F0WJMfVWB&X-Amz-Signature=dbc600f6609fe9490a7565ba07473ca2fe9f53e371e9970289789a6ab524626b&X-Amz-SignedHeaders=host&x-id=GetObject)


### 02 


	```c++
	#include<iostream>
	using namespace std;
	int main(){
	    int num1, num2, num3;
	    cout << "Enter num1: ";
	    cin >> num1;
	    cout << "Enter num2: ";
	    cin >> num2;
	    cout << "Enter num3: ";
	    cin >> num3;
	
	    if (num1 > num2){
	        if (num2 > num3){
	            cout << "The small one= " << num3;
	        }
	        else if(num2 < num3){
	            cout << "The small one= " << num2;
	        }
	        else{
	            cout << "num2==num3";
	        }
	    }
	    else if(num1 < num2){
	        if (num1 > num3){
	            cout <<"The small one= "<< num3;
	        }
	        else if(num1 < num3){
	            cout << "The small one= " << num1; 
	        }
	        else{cout << "num1==num3";}
	    }
	    else{
	        if (num2>num3){
	            cout <<"The small one= "<< num3;
	        }
	        else if(num2<num3){
	            cout << "num1==num2";
	        }
	        else{
	            cout << "SAME";
	        }
	    }
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/99a9a375-20ab-49b3-bc98-de5e7d638e36/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466SFI42IYS%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044758Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJGMEQCIEF9ezLSUx%2BVzxW6S2x1eQ948TSMXU4RhpjqTnLthRS%2FAiBPlBpjESIMEPdJuw6Nvfj3B4NVPt6%2Bi8ofq72AVq7z2CqIBAid%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAAaDDYzNzQyMzE4MzgwNSIMLxQstuchcaCKx9BLKtwDRel%2BMJX%2BEVXe9ECBVoTK50Gic4Ea4LpxbTbcsK6ug388Ebr6In1ETe2%2B%2FkXeXrfpDvFA8dq2j69irZ3bD1ojs53mlTEnKW8yn2dBGB45PfVrODBOFkXTErEtmMwmoSzsrS75ziyXcKgykWLiTRZj0KkKctSB4Yr7kRZnBV0DR4fRLPBpOwaBa1mD0k5nLau1P7MUmMbBwWA41kw7UP3rUXkliYdn0JJvIeGbwhX%2FlDmBPBu%2FQ%2F49TAdTIkeHzcyJZDf2w9BnX4p8wcVd6Bymra%2FmY9cpzAIdfsoaYUtnw3r8I4R%2FfojtgFlaY99ZqVQRbd2VO%2BGOkNwfP2sLP8Mz%2BTuniU3DBvYlsUZu9HUQ55cjpXBVfu92wbIkB2Ea9uFd5zpmZD6AKFSeP32y311tM%2B%2BYaitGtkGkYRXViWzxDN3y2P2F5x%2FNEgIfkkk71pGQmMynnLbqblrPrUxZzDjtYHd5Z8wEoUjasmsf5gywKsvvlX5Cn4wUkE2oxsqQ3l1lnkwXCgwDukDCfTbukH0i1Cmwst9n46fnNUJ7qgFepuuQT9FtgWuin1lL%2FMq3z1rwuM6JtOzr55JKaBrX6PnsDeXshpmutgAXFORKZcmR8BC8FneCBtjZtMW8CD4wht7kwQY6pgE8Zi6pBZ7K3r1R%2Fj9PqgCoqz2HD820uBw%2FOzuvjKy5h%2BYGMZ7wx4F6xa66KifBLDvFRyfk9%2BKbdA7TLeD%2FuvucsLA%2BJSx3C70q6aTLdt0IXn%2BQbF69zp0mp%2BSZLq2M9vuqsVx8YmDC1qrn8IC95Ii0QgHeHNclPetGOT0Bl46Eitjz10c1tDdzTbKyX0RnQtL6GYbF0kVEYskyLND4piMYfmL7FvqT&X-Amz-Signature=141222aa4cb5bb2dbe45eafd9243820fb660d7d65df845f099d2f695210d7ae5&X-Amz-SignedHeaders=host&x-id=GetObject)


### 03 


	```c++
	#include<iostream>
	using namespace std;
	int main(){
	    int num;
	    cout << "Enter integer(1-12): ";
	    cin >> num;
	    switch(num){
	        case 1: cout << "Jun.";
	            break;
	        case 2: cout << "Feb.";
	            break;
	        case 3: cout << "Mar.";
	            break;
	        case 4: cout << "Apr.";
	            break;
	        case 5: cout << "May";
	            break;
	        case 6: cout << "June";
	            break;
	        case 7: cout <<"July";
	            break;
	        case 8: cout <<"Aug";
	            break;
	        case 9: cout <<"Sep";
	            break;
	        case 10: cout <<"Oct.";
	            break;
	        case 11: cout <<"Nov.";
	            break;
	        case 12: cout <<"Dec.";
	            break;
	    }
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/90f68e45-4550-4ec6-9556-af335454a057/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB46643RV2NZE%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044758Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJIMEYCIQDkw5Q7juaEsVnieeVvwYtOD6tweix4WSdxJvaY%2Fr8LlgIhAOZ1okdHFinSOnDhJWybhcoddKeKhb4oW4qp6MwYQ2CZKogECJ3%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEQABoMNjM3NDIzMTgzODA1IgyqZRSe39dxLro9ePQq3AMzgLApiznRKtVPbWaKqr8Ikrw7LjKdzxZo3VpDMEB5YP7y75veQkTLqe7Kl%2B%2FHDF%2F0F0fEeGFlWg%2FXRmtAYV85prqFrnuhHd4u%2FhuiIlaF4lkh1BSduyW5FD8U9O6X7k5kDPVUlHqbMzscFgYduSaEee4PbxpPyX9EM5EoB%2Fppi5YShc9dONmSpAGt117a7YriqyFkAue%2FvkZ1flaAIuKRNhL90MWNnWX1QRouJtX77nqTLcLfDEmxRDHuX5l90PSAWPb2QUHBzAdxOb4eZFAUDsy%2Bf5eJXVRwzbeJpgtrg27V0VUyaM7OhGIv4Vo0XF550tyzct6OXm5PYAv%2BcAB%2BMaPpCYiu0t3pjvk9d6D2aojsxAnwXYA5kUhtaGQigto5h4NtygT19WhjQcAF2uE0TB1sJcSsaHSR0fQQM339XOvq1V3w%2BcUqJD8SPNYolGAqtxKwYKFKlncULk0g9VCV8B3v3EEnU8DhuyntjqxU3I0WfWbSBi5c8RqA9%2BJMUj6REfED7euO2Mce0lpE2mDVRoeMXeSRKMRB9JQKlI7ia3AUo%2FKW8722D%2F3060%2FcBcNFqIJZv3%2BSH3uGkvHxbfqPxSOAHMbwOKE6l234oXnAkMf%2B%2BWwXLtDj9tTsSTDE3eTBBjqkAUDjsoXTBCugxeA%2Fv6t4twxDk0db1djX%2FtFFBw%2Bm3Sip%2Ff5wwvS9IHZF%2Fjh05ZUvIttoJ3xH8WI%2BRTk7bypDQLD2sP1b%2FzEMTb8%2B474pF5grbwgafXeIvkQFHtP40xhtkIs5VBj7in0J6cp9OZXsS9CxWJJc6WHI2jXt69PWU0uYCqpmldtuFGhTc26AKpqrAxe2%2FncemREuReUt5%2BYbtv9hv%2FO8&X-Amz-Signature=7158fe3de3f0daaea963182b41495a2a264c60ff393598faf0bbb66c6c2d0580&X-Amz-SignedHeaders=host&x-id=GetObject)


### 04 


	```c++
	#include <iostream>
	using namespace std;
	int main(){
	    char car;
	    int hour;
	    cout <<"Enter the type of car(c, b, t): " ;
	    cin >> car;
	    cout <<"Enter the parking hour: ";
	    cin >> hour;
	
	    switch(car){
	        case 'c': cout << "Parking fee= " << hour*2 <<" dollars.";
	            break;
	        case 'b': cout << "Parking fee= " << hour*3 <<" dollars.";
	            break;
	        case 't': cout << "Parking fee: " << hour*4 <<" dollars.";
	            break;
	    }
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/e3dfaae1-76b2-4af5-bd5d-6147d432145f/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB4662MZAULOF%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044759Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIBUCyoI6zjt6lPQgg%2FsVBsmhjQfmcVfq%2BdqgFG2bxGrOAiEAoiNiMwOOiUCPVfdu%2BkY%2BEL0ku9aTGOwCIVLHM3gTg4wqiAQInf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDKqbNl5mfzrfFaSNYyrcAwfuGLUY1Ilnjzm%2FzU3NFKiyDc5f87iqaTqRSR9rnayq2lpvlsVMIOYRLEyplaiLkJGi4cJEzSIuCtiR07ZLWHo19zZp3Sbbzsvv5THzW4nUfbZuGMV%2Fq4nG8PwyvI1HL3dh6U2DstEdH2bO2Tt9cHoCd90YzgMUqP0bIgdJL2mVQcXmHJT9WHD94ufjmWSjq3xK1tdYc2rnbwiRQL0j4MGLcVjVVgR%2Bn0wu6hBINlGEKV1aty5jSoM%2B85xZNyyHj4ccdzUWwBuXsTWZ4I97jvvqbWW45X7P6fMW8xm%2BDByZTW7EOhOB%2Fvih9e0YH5U39lQvaTDwxkSvXvbqOqHDIwNCnTpXoEEX80C3lukCbNP2kRo9AkVnDPGeutaeu%2FTvCkG%2FW8uvDy%2FLIslcO2br%2FPCDzwnVAb5QKWHGcADXDjnVS5Jg2kt6D3yo7jBPgJA3sFFARIzCTN2aDThTHwxGlQ%2FmwImXijUL0pl%2FKDkMQ%2BvLS6lUpwkw21b4Va9Uz1Y7ZPV%2Fe4Onq9vkiaPraxJBp1XoqWGiE3C73J9pTPrW2CSRLsLgmqwVg9DFrnuisDOSCO7bLd59tSBXorWpjz0me92mqLn5kMhbcSPvE3I3L9CSpYI52Tv6S%2BaFaAwOMPLd5MEGOqUBK5Vl9JGCJgc3duT5BlYJg2KEjSVSH80XchBqZuy4fc8%2BkNb2ft1Zvrnv0tcig%2FDV1Xg0UfkOoUsc15tJg3TP%2BZ%2BP8%2FU9DMRqsSTzohESc7uDI7WcJ9pU167vwYh7omkx46kHEzwgT%2BVU%2BErn1TEwruZmO9b%2F9BZxWifVTm%2BbWsSf0I7rxEsdjtRV2ZjFXOCFEAxb41aKecNhdtEIa9msPpPV2m8u&X-Amz-Signature=901fcde5f0a65e56239549de4ccbc4004d5a8ec8f62ee1412766e4227924347d&X-Amz-SignedHeaders=host&x-id=GetObject)


### 05 


	```c++
	#include<iostream>
	using namespace std;
	int main(){
	    int score1,score2,score3;
	    char grade;
	    cout << "Enter scores: ";
	    cin >> score1;
	    cin >> score2;
	    cin >> score3;
	
	    float mean = (score1+score2+score3)/3;
	
	    if (mean>90){grade='A';}
	    else if(mean>80 && mean <=90){
	        if(score3>90){grade='A';}
	        else{grade='B';}
	    }
	    else if(mean>70 && mean <=80){
	        if(score3>80){grade='B';}
	        else{grade='C';}
	    }
	    else if(mean>60 && mean <=70){
	        if(score3>70){grade='C';}
	        else{grade='D';}
	    }else if(mean=<60){
	        if(score3>60){grade='D';}
	        else{grade='F';}
	    }
	    cout << "Mean: " << mean << endl;
	    cout << "Grade: " <<grade;
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/295beb37-4966-499c-87c3-fd74f37a2bb3/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466SOTOLSIF%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044800Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJGMEQCIFaRoi2dzkTJDpGcOnDi0XC16nwhOs9YkhezBJhSC9IyAiB5vJvx2WVoVpPWyTSCBp64c0vnGqM5VuhOCS82yLrBWyqIBAid%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAAaDDYzNzQyMzE4MzgwNSIMIBYaYAiBAXoAYIk6KtwDlRTUC03DD4bKr1RBibsE6nfAsKqkvUqJ7mRnbgi%2FrvYHcQRpvzDt61Jp5pUeUYmGiXm0SAVJUubuBfGGiVj7dnvbTWS%2BKsT5VZ%2FOJV6Pvw7AvzyvyGCt4PTW80aAlyKHf390DfjWC4XJACaeJ9u0aRaVEot%2FtGJf8rPoYSg31A3Rkt%2B5BL5esY4unjnC0J3b4YsTc%2F3PiV36BWd%2FOJ7nMFRf7TfW2THXcs8VSUai%2Bxp9dihM22ysQSxWFavU77DkKh73BvfnbWxX0uT4QwcyuP%2FwADCLxYz6PncYL2%2B%2FAekpPjLmFPQ2TuPl4Dx8F2%2FvARQg0RIEiNZh0sr1xfhPiSErV%2BOb6dzPb3pgoakVjH7FMTXT6F%2FweTaHlRS5bpfPDc%2F0SZ5YC0Cf9TNNuTTlBsQaszad58WWaC3NuRj4Wra0IhbPXPMVhEyhl5p9jEcnOI05P5DN8U8jK2R%2BVdo%2B3TuWKtXbuGNqGz0m1FmTQzw8G%2Fc%2FtgeSFKLydnzRomksQ9w4r5dnqqZD2Ffu7X7PnV7cvwKyZkUC6EIurc3zqnqo33XAfUgaE0J9eW9oWZMcxwe3plGWhGPtLDoPzZStaqk9%2FwM3n2muNWDT7qmjEU9z6SjmVrmjouu%2F2BAw1d3kwQY6pgGDNaL5hcloVAC0YLauTSMQYI6iQAfMq%2Bff5sFa%2FpzdpPF5miDZhY4494dFO6ibeR6eO1kGzqDKPVPv0cX3REzAjIybFzYDM3ZLf%2BnFnED2x5qg5JAWUYkO6dBywEomBU31hcXy3e6luL0OvrD5fo6%2Fq8GYxdl2XWlHeNujCGJxCqE1seRveVOy%2BaOBjqM96xa9STAC%2FzFbssYyqtPXLEGFdJFaR4p3&X-Amz-Signature=f8e77615eccf5e986f57152fe76a5f4e72b111c832ed13682e83d98435c93336&X-Amz-SignedHeaders=host&x-id=GetObject)


### 06 


	```c++
	#include<iostream>
	using namespace std;
	int main(){
	    int lecture;
	    cout << "# of lectures(0-12): ";
	    cin >> lecture;
	    if (lecture>12){
	        cout << "tuition fee= " << 12*10 <<" dollars.";
	    }
	    else{cout << "tuition fee= " << lecture*10 <<" dollars.";}
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/e52d4f97-4640-4929-b060-8899fe6fe1d6/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466WLZ7X5F2%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044800Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJGMEQCIEvusTebNdproWtUYjTz%2FuiI%2FZZWtv0RwxSIL%2FyhFn9hAiAxhmMbAT6%2F5etafea1lRvWhPF88IvPRs0A8ybANeW2YyqIBAid%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAAaDDYzNzQyMzE4MzgwNSIMW2rMJhr567hrptj2KtwDGLfc1RmQMGFvzFRxqK8t60bjkJw2ZLN%2B8ZJhK1qOZEMTmMMzh20UdMcZSYJsKsFgmMRb%2B0TFVUyKiXvZvtersy0dTPApqCh5P229e%2B96G3KdMSI%2B6cSoFiw6KsRLCuAJF%2FA9CP2M3tS%2FPHYil0hSe0wRrDteDgH9WlZu2FPSGWCVQigSNe9NhMBGKDoioQQP8%2BlyhfcE%2BD6YfL9W%2Faiha4eEKTfWOWb8x5C5FJzRNa%2FA%2B2k9cgT0VPP3hE2oIReUegPX1T%2FDFsQIrhzomDLhrdnBqG47bAwT%2F4w%2Fbtkn8TJHAy6f%2BmUFtPqiTiEV%2F41MdDXwO3U%2BDUski0eibVV8KS63AgDfghk3o7C2Hb6wMFwd5GvyStWwiQNMmoQNF6TTrzDCRKMN9x74kzpA320HWd6yMK7R0rMgMBw%2FmndxXwboy%2Fd%2ForINxAtTwtp9lwmcStO27gONAOPBN%2Fa7x%2BoWzjv4SCf0W%2B7q2Yyn5BC%2FtDf0Ex11J2M34mYwxEFNqdi6cRXmWekKuiTHbym%2FwPXCDB80J3bJhWk46U0wzoIIM9HwDljp%2B1apXOKsgfCg54YrWiTJNAobA3eZYc8PVgY08IFTUgM7Jm1Mpl%2F4ddFoplaS%2F3Rt%2BmjEpBZ7KR8w3uLkwQY6pgHpv5ZjkGJ7QqH0AKN3EnoyGcV3RpNkJke6CJvRZyLUtsDhnAM%2BzrS8KwlCu8xfKMms2ooydKtxCDFB9k3gl3dos5umK0D8logJlZQdi%2B3wyrHkRmYh0a48bSTsjtVyZozQp%2BXKIMbgI7BT14UsoA86Do%2B36pKRGl%2Bd97ozsTiIf0s20N7JYr3wN8wtwXNhGqnBM649aOHeE2wg06oP0bGQjNK%2FnyUf&X-Amz-Signature=5b5096360353ddc4afcf28d9afd158a6b3609a76fb9570bb7a77119973139c9a&X-Amz-SignedHeaders=host&x-id=GetObject)


### 07 


	```c++
	#include<iostream>
	using namespace std;
	int main(){
	    int count;
	    float cost;
	    cout << "Enter count: ";
	    cin >> count;
	    cout << "Enter cost: ";
	    cin >> cost;
	    if (count>=1 && count<=9){
	        cout << "Total cost= " <<count*cost <<" dollars.";
	    }
	    else if (count>=10 && count<=49){
	        cout << "Total cost= " << count*cost*0.97 << " dollars.";
	    }
	    else if (count>=50 && count<=99){
	        cout << "Total cost= " << count*cost*0.95 << " dollars.";
	    }
	    else if (count>=100){
	        cout << "Total cost= " << count*cost*0.90 << " dollars.";
	    }
	    return 0;
	}
	```


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/d4cf4a6e-057e-4fcd-8c10-4596c944ac02/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466WCKJXD7D%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044803Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIQDSdNHfkmtmzuipCTFsuGMxkUTqBiphxPDgukmOejeztAIgLV6GPhel9rMJAGoOHYUNu6rR4LhfcL25LZtzNZrsKPsqiAQInf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDPDf3wzHh%2FEwUUhR3ircA21V1vG9BBV4i3pYIHXxp3xHHaMrjlPHfL0hsTzXFCg1JBFAe3W1MjA9iqpNOTG4LO3jwdUmPfr3Djzq0uPn3MM89VYAV8int5yBsCG6yJ1sFaF2JAxlvBm3z%2FKkCeGzDMCziZrSAJPdILfTBVXZQ5GD4Cm5Zy5pAF7Z7QSEM%2FOJuewxis%2BnaQzhFCo%2BMz4OQjMEDxB7lzqLJihEyMpJKWRWfiIxTjbx2MiVk%2BT8waDGZY5ePlRi%2F%2FN1qjND197n30Dbg3AiItGtlC9xiN7GkSfyLc9JVbcBSQSVyEVQP2mk0dulzoiho0yAbYn3L03xyikuRVnSSaE8tt%2BXU205wxSDPK5tTpVcRZPlDjxBcj%2Fy78AM27dQ3RKF70zMfzvo0e%2Fh8Puo7gRF73HhNJ4RyhCnyUtvn3Ld5Od05itznt5g5yoGIXM2pR6tNVCNYYpLQ1GV3fsMr%2FXZ%2FJ2J9tY3nyS8tNEv5QlU4OTq2%2FXpsvdyvrgrfwVJfIWn0Yw12xr7IId4ZrHJ9SqJXptrTtrfFz47ruUVrjABhYSMQkn7apJ2cgxshaiX0ldLU7knyoqAtZP6WurcF70wEl2bVmhOOg6JRzWFkcwT15pjY5J%2B8N4VBc8P2zKOdfJOXe72MOHd5MEGOqUBdfC5yksOAPLowrMksMfolkKZEivHQlcCRlVls4v%2Fz8SZAW1LGFqaPII2lxgv%2F9e5PnpWjLX0%2Bszys%2Fn8MccXbqIlTy0qanr02LiBnp5YCjlfR8pkE5P2pYbWLDgqsYlG0biiw566m2eRiASlSN6PV886zFQcioxawtTqtYe0w4y9R2dbMu6LOMhYbb1Rt9PPCaE6z%2B2IsbgUbMI755DYM3jif38P&X-Amz-Signature=432f20baf5bfd36408e1ea91fb7893b9ebe8c598a4611de0c791bc5ba8c30b9a&X-Amz-SignedHeaders=host&x-id=GetObject)


	![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/dd066649-1ca9-4db7-aa53-e132f4b7807d/be9ce8c9-4d51-4a27-ad64-3e53b43e559c/image.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=ASIAZI2LB466WCKJXD7D%2F20250530%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20250530T044803Z&X-Amz-Expires=3600&X-Amz-Security-Token=IQoJb3JpZ2luX2VjENT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLXdlc3QtMiJHMEUCIQDSdNHfkmtmzuipCTFsuGMxkUTqBiphxPDgukmOejeztAIgLV6GPhel9rMJAGoOHYUNu6rR4LhfcL25LZtzNZrsKPsqiAQInf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAAGgw2Mzc0MjMxODM4MDUiDPDf3wzHh%2FEwUUhR3ircA21V1vG9BBV4i3pYIHXxp3xHHaMrjlPHfL0hsTzXFCg1JBFAe3W1MjA9iqpNOTG4LO3jwdUmPfr3Djzq0uPn3MM89VYAV8int5yBsCG6yJ1sFaF2JAxlvBm3z%2FKkCeGzDMCziZrSAJPdILfTBVXZQ5GD4Cm5Zy5pAF7Z7QSEM%2FOJuewxis%2BnaQzhFCo%2BMz4OQjMEDxB7lzqLJihEyMpJKWRWfiIxTjbx2MiVk%2BT8waDGZY5ePlRi%2F%2FN1qjND197n30Dbg3AiItGtlC9xiN7GkSfyLc9JVbcBSQSVyEVQP2mk0dulzoiho0yAbYn3L03xyikuRVnSSaE8tt%2BXU205wxSDPK5tTpVcRZPlDjxBcj%2Fy78AM27dQ3RKF70zMfzvo0e%2Fh8Puo7gRF73HhNJ4RyhCnyUtvn3Ld5Od05itznt5g5yoGIXM2pR6tNVCNYYpLQ1GV3fsMr%2FXZ%2FJ2J9tY3nyS8tNEv5QlU4OTq2%2FXpsvdyvrgrfwVJfIWn0Yw12xr7IId4ZrHJ9SqJXptrTtrfFz47ruUVrjABhYSMQkn7apJ2cgxshaiX0ldLU7knyoqAtZP6WurcF70wEl2bVmhOOg6JRzWFkcwT15pjY5J%2B8N4VBc8P2zKOdfJOXe72MOHd5MEGOqUBdfC5yksOAPLowrMksMfolkKZEivHQlcCRlVls4v%2Fz8SZAW1LGFqaPII2lxgv%2F9e5PnpWjLX0%2Bszys%2Fn8MccXbqIlTy0qanr02LiBnp5YCjlfR8pkE5P2pYbWLDgqsYlG0biiw566m2eRiASlSN6PV886zFQcioxawtTqtYe0w4y9R2dbMu6LOMhYbb1Rt9PPCaE6z%2B2IsbgUbMI755DYM3jif38P&X-Amz-Signature=af132de31af7b563182b2b07e8365254d09a397bcf327974a978606a330a6bec&X-Amz-SignedHeaders=host&x-id=GetObject)

