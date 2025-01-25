#include<stdio.h>
void prime(int n){
    int count=0;

    if(n<=1){
        count=1;
    }
    else{
    for(int i=2;i<n;i++){
        if(n%i==0){
            count++;
            break;
        }
    }
    }
    if(count==0){
        printf("prime");
    }
    else{
        printf("not");
    }
    
}
int main(){
    int n;
    printf("Enter n: ");
    scanf("%d",&n);
    prime(n);
    return 0;
}
