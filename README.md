# palindrome-number
#find palindrome number
#include <stdio.h>
#include <stdlib.h>

int main() {
    int n, n1, reverse = 0, remainder;
    
    printf("Enter number:");
    scanf("%d", &n);    
    n1 = n;
    
     while (n > 0){
        remainder = n % 10;
        reverse = reverse * 10 + remainder;
        n = n / 10;
    }
    
    if (n1 == reverse){
        printf("\n number is a palindromic number\n",n); 
    }
    else{
        printf("number is not a palindromic number\n",n); 
    }    
    return 0; 
} 
/*OUTPUT:
Enter number:121
number is a palindromic number
*/
