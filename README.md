# cce-0409
## 進階題：迴文判斷
```C
#include <stdio.h>
int main ()
{
	int n;
	scanf("%d",&n);
	int a=n/1000,b=n%1000/100,c=n%100/10,d=n%10;
	if(a==d&&b==c)
	printf("YES\n");
	else 
	printf("NO\n");
	}
```
## 函數反序排列數字
```C
#include <stdio.h>
int f(int n)
{
	int p;
	int m=0;
	
	while(n>0)
	{
		p=n%10;
		n=n/10;
		m=p+m*10;
		}
		return m;
		}
		int main ()
		{
		 int n,m;
		 scanf("%d",&n);
		 printf("%d\n",f(m));
		 }
```
## 進階題：陣列找出現次數 
```C
#include <stdio.h>
int main ()
{
	int a[50],i,n,x;
	int count=0;
	for(i=0;i<10;i++)
	{
	scanf("%d",&a[i]);
	if(a[i]==0)
	break;
	}
	scanf("%d",&x);
	n=i;
	for(i=0;i<n;i++)
	{
	if(a[i]==x)count++;
	}
	printf("%d\n",count);
	}
  ```
  ## 進階題：判斷大小 
```C
#include <stdio.h>
int f(int a,int b){
	if(a<b) return -1;
	else if(a==b) return 0;
	else return 1;
}
int main(){
    int a, b;
    scanf("%d %d", &a, &b);
    printf("%d",f(a,b));
    return 0;
}
```
## 進階題：計算一列整數的總和
```C
#include <stdio.h>
int main ()
{
	int sum=0,a;
	while(a!=999)
	{ printf("Enter an integer ( 999 to end ): \n");
	scanf("%d",&a);
	sum+=a;}
	printf("The total is: %d",sum-999);
	}
```
