# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
      #include <stdio.h>
      
      #include <math.h>
      
      
      void calculateEMI(float principal, float rate, int time) {
      
          float monthlyRate = rate / (12 * 100); // Monthly interest rate
          
          int months = time * 12; // Time in months
          float emi;
      
          emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / 
                (pow(1 + monthlyRate, months) - 1);
      
          printf("Monthly EMI is: %.2f\n", emi);
      }
      
      int main() {
          float principal, rate;
          int time;
      
          printf("Enter loan amount (principal): ");
          scanf("%f", &principal);
      
          printf("Enter annual interest rate (in %%): ");
          scanf("%f", &rate);
      
          printf("Enter loan period (in years): ");
          scanf("%d", &time);
      
          calculateEMI(principal, rate, time);
      
          return 0;
      }


## OUTPUT
![image](https://github.com/user-attachments/assets/365f0277-f752-41b2-b882-9928c9f7ddbb)






## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
    #include <stdio.h>
    
    void generateFibonacci(int terms) {
        int a = 0, b = 1, next;
    
        printf("Fibonacci series for %d terms:\n", terms);
    
        for (int i = 1; i <= terms; i++) {
            printf("%d ", a);
            next = a + b;
            a = b;
            b = next;
        }
    
        printf("\n");
    }
    
    int main() {
        int terms = 6;
        generateFibonacci(terms);
        return 0;
    }


## OUTPUT
![image](https://github.com/user-attachments/assets/b14342cf-f890-497a-a88e-df0327e51783)









## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
     #include <stdio.h>
     
     int main() {
     
         int n;
     
     
         printf("Enter number of elements: ");
         scanf("%d", &n);
     
         int arr[n];
     
         
         printf("Enter %d elements:\n", n);
         for (int i = 0; i < n; i++) {
             scanf("%d", &arr[i]);
         }
     
         
         printf("Last element of the array: %d\n", arr[n - 1]);
     
         return 0;
     }


## OUTPUT


![image](https://github.com/user-attachments/assets/7f0d2321-7a6f-473f-a2cb-d1d6cbe5b0b4)







## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
      #include <stdio.h>
      
      int main() {
      
          int n, count = 0;
      
         
          printf("Enter the number of elements: ");
          scanf("%d", &n);
      
          int arr[n];
      
      
          printf("Enter %d elements:\n", n);
          for (int i = 0; i < n; i++) {
              scanf("%d", &arr[i]);
      
      
              if (arr[i] > 0) {
                  count++;
              }
          }
      
      
          printf("Total number of positive elements: %d\n", count);
      
          return 0;
      }



## OUTPUT
![image](https://github.com/user-attachments/assets/569efba3-c27c-4357-82d1-0de16de54471)






## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
      #include <stdio.h>
      
      int main() {
          int n;
      
          
          printf("Enter the number of elements: ");
          scanf("%d", &n);
      
          int arr[n];
      
      
          printf("Enter %d elements:\n", n);
          for (int i = 0; i < n; i++) {
              scanf("%d", &arr[i]);
          }
      
      
          printf("Array after replacing even elements with 'E':\n");
          for (int i = 0; i < n; i++) {
              if (arr[i] % 2 == 0) {
                  printf("E ");
              } else {
                  printf("%d ", arr[i]);
              }
          }
      
          printf("\n");
          return 0;
      }
      

## Output:

 ![image](https://github.com/user-attachments/assets/bdc900aa-5922-40dd-8f9e-fcb574508b7f)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



