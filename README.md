#include<stdio.h>
#include<string.h>
#define MAX 256
int main(){
    char s1[100],s2[100];
    int count1[MAX]={0},count2[MAX]={0};
    printf("enter the string1 ");
    scanf("%s", &s1);
    printf("enter the stirng2 ");
    scanf("%s", &s2);
    if(strlen(s1)!=strlen(s2)){
        printf("Not Anagram");
        return 0;
    }
    for(int i=0;i<MAX;i++){
        if(count1[i] !=count2[i]){
            printf("Not Anagram");
            return 0;
        }
    }
    printf("Anagram\n");
    return 0;
}
