#include<stdio.h>
int checkpalindrome(int n);
int main(){
int num;
printf("enter a positive number: ");
scanf("%d",&num);
if(checkpalindrome(num)){
    printf("%d is a palindrome number",num);
}
else{
        printf("%d is not a palindrome number",num);

}
return 0;
}
int checkpalindrome(int n){
int orginal=n;
int reversed=0,remainder;
while(n!=0){
    remainder=n%10;
    reversed=reversed*10+remainder;
    n/=10;
}
return(orginal==reversed);
}
# c-palindrome-number
