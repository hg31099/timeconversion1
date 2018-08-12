#include<stdio.h>
#include<string.h>
char* abc(char ch[])
{
    if(ch[8]=='A')
    {
        if(ch[0]=='1'&&ch[1]=='2')
        {
            ch[0]=0;
            ch[1]=0;
        }
        return(&ch[0]);
    }
    else
    {
        if(ch[0]=='1'&&ch[1]=='2')
        {
            return(&ch[0]);
        }
        else
        {
            int a;
            a=ch[1]+12;        
            ch[1]=a%10;
            ch[0]=a/10;
            return(&ch[0]);
        }
    }
}
int main()
{
    int ch[15],i=0;
    gets(ch);
    char *t;
    t=abc(ch);
    while(*(t+i)!='A'||*(t+i)!='P')
    {
        printf("%c",*(ch+i));
        i++;
    }
    return 0;
}
