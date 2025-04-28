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
```#include <stdio.h>
#include<math.h>
float EMI()
{
    float p,r,t,emi;
    scanf("%f",&p);
    scanf("%f",&r);
    scanf("%f",&t);
    r=r/(12*100);
    t=t*12;
    emi=p*r*pow(1+r,t)/(pow(1+r,t)-1);
    printf("Monthly EMI is= %.3f",emi);
    return 0;
}
int main()
{
    EMI();
    return 0;
}
```


## OUTPUT


![image](https://github.com/user-attachments/assets/ce6e9cf4-e81c-43aa-a2f2-115feb3f5759)



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
```#include <stdio.h>

int main() {
    int n = 6;
    int first = 0, second = 1, next;

   
    printf("Fibonacci series up to %d terms: \n", n);
    printf("%d %d ", first, second);  

    for (int i = 3; i <= n; i++) {  
        next = first + second;  
        printf("%d ", next);
        
        
        first = second;
        second = next;
    }

    printf("\n");  

    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/04fda13b-9c3d-49fd-87b0-204f13ecbc1f)







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
```
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
        
    }
    for(i=0;i<n;i++)
    {
        
            printf("%d ",a[i]);
            
        
    }
    return 0;
}
```

## OUTPUT


![image](https://github.com/user-attachments/assets/8b46117a-ba7b-4bcf-9ac5-cbb55e084975)







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
```#include<stdio.h>
int main()
{
    int a[100],i,n,c=0;
    scanf("%d",&n);
    for(i=0;i < n;i++)
    {
        scanf("%d",&a[i]);
    }
    for(i=0;i < n;i++)
    {
        if(a[i]>0)
        c++;
    }
    printf("count  of positive numbers  in array: %d\n",c);
    printf("count  of negative numbers  in array: %d",c);
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/de5b9706-dbb4-4b86-8af0-d1e21af54482)




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
```#include <stdio.h>

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
```
## Output:
 
![image](https://github.com/user-attachments/assets/794333a7-3137-4f85-bea0-ee93a4e0c053)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



