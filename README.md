# Sum of K consecutive integers
#include<stdio.h>
#include <stdlib.h>

int main()
{
long long int n,k,a[100001],sum,i,j,count=1;
scanf("%lld",&n);
for(i=0;i<n;i++)
{
    scanf("%lld",&a[i]);
}
scanf("%lld",&k);
sum=0;
for(i=0;i<n-(k-1);i++)
{
    j=i;
    while(count<=k)
    {
        (sum)=(a[j])+(sum);
        j=j+1;
        count++;
    }
    printf("%lld ",sum);
    sum=0;
    count=1;
}

}
	
