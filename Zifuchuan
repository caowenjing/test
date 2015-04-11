#include <iostream> 
 
using namespace std; 
 
void myReverse(char*, char*); 
char * senReverse(char*); 
int main() 
{ 
    char sen[]="hello, I am a student!"; 
    char *result=senReverse(sen); 
    cout << result << endl; 
    return 0; 
} 
void myReverse(char *start, char *end) 
{ 
    char temp; 
    while(start<end) 
    { 
        temp=*start; 
        *start=*end; 
        *end=temp; 
        start++; 
        end--; 
    } 
} 
char * senReverse(char *sen) 
{ 
    char *start=sen, *end=sen+strlen(sen)-1; 
    myReverse(start, end);  //先反转整个句子 
     
[cpp]
释部分是另外一种实现，只不过看起来有些繁琐
int loc;  //记录每个单词的长度
for(start=sen,end=start;(*end)!='\0';start+=loc)
{
    loc=0;
    while((*end)!=' '&&(*end)!='\0'){end++, loc++;}
    end--;
    myReverse(start, end);
    end+=2;
    loc++;
}
*/ 
end=start; 
while(*start!='\0') 
{ 
    if(*end==' '||*end=='\0') 
    { 
        myReverse(start, --end); 
        if(*end=='\0') 
            break; 
        end+=2; 
        start=end; 
    } 
    else 
        ++end; 
} 
 
return sen; 
