#define _CRT_SECURE_NO_WARNINGS 
#include<stdio.h>

int main() {

   int a, b, c;
   int total;
   int max;
   
   scanf("%d %d %d", &a, &b, &c);
   
   if ((a == b) && (b == c)) {
   
      total = 10000 + (a * 1000);
      printf("%d", total);
   }
   else if ((a == b) || (a==c)) {
   
      total = 1000 + (a * 100);
      printf("%d", total);
   }
   
   else if ((b == c)) {
      total = 1000 +(b * 100);
      printf("%d", total);
   }
   else {
   
      if (a > b && a > c) {
         max = a;
      }
      
      if (b > a && b > c) {
         max = b;
      }
      if (c > a && c > b) {
         max = c;
      }
      
      total = max * 100;
      printf("%d", total);
   }
   return 0;
}
