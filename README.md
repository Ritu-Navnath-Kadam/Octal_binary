# Octal_binary
#include<stdio.h>
int deci(int ans);

int deci(int ans)
{
    int l,a,p=1;

    while(ans>0)
    {
        l=ans%2;
        a=a+(l*p);
        p*=10;
        ans/=2;
       
        
    }
    printf(" Binary number =%d",a);


}

void main()
{
    int on,ritu,ld,power=1,ans=0;
    printf("Enter octal number :");
    scanf("%d",&on);
    
    while(on>0)
    {
        ld=on%10;
        ans=ans+(ld*power);
        power*=8;
        on/=10;
    
    }
    printf(" Decimal number = %d\n",ans);
    
    deci(ans);


}
