#include<bits/stdc++.h>
using namespace std;
#define symbol "."
int main(){
    bool flag = true;
    int count=0;
    char ip[]="0.123.123.2";
    char *token;
    queue<int> q;
    
     int len = strlen(ip);
     cout<<len<<endl;
    for(int i=0;i<len;i++)
    {
         if(ip[i]=='.')
         count++;
    }
    
    token = strtok(ip,symbol);
    
    while(token!=NULL){
        q.push(atoi(token));
        
      token = strtok(NULL,symbol);
    }
    
   
    while(!q.empty()){
        if(q.front()>255)
        flag=false;
        
        q.pop();
    }
    
    if(count==3)
    flag = true;
    
    else 
    flag=false;
    
    string j = (flag==true)?"YES, VALID":"NO, NOT VALID";
    cout<<j;
    return 0;
}
