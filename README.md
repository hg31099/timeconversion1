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
    int ch[15],i=0;#include<stdio.h>
#include<string.h>
char ch[11];
char* abc(char ch[])
{
    if(ch[8]=='A')
    {
        if(ch[0]=='1' && ch[1]=='2')
        {
            ch[0]=48;
            ch[1]=48;
        }
        return(&ch[0]);
    }
    else
    {
        if(ch[0]=='1' && ch[1]=='2')
        {
            return(&ch[0]);
        }
        else
        {
            int a;
            
            a=(int)ch[1]+ (ch[0]-48)*10-36;
        
            ch[1]=a%10+48;
            ch[0]=a/10+48;
            return(&ch[0]);
        }
    }
}
int main()
{
   char ch[11],i=0;
    gets(ch);
    char *t;
    t=abc(ch);
    while(i<8)
    {
        printf("%c",*(t+i));
        i++;
    }
    return 0;
}

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
