
Mohamed Gamal

Sec 2 - BN 12 - 9210954
 

## **The Fibonacci Sequence Problem**
The fibonacci sequence is a series of number, where a number is the sum of the two numbers laying before it in the series.
You can find out more about it [over here.](https://www.omnicalculator.com/math/fibonacci#what-is-the-fibonacci-sequence)

We will be covering:
 

 - Using Recursion To Solve The Fibonacci Problem
 - Using Binet’s formula To Solve The Fibonacci Sequence Problem

 <a href="https://ibb.co/fk5jq44"><img src="https://i.ibb.co/fk5jq44/Leonardo-Pisano-Fibonacci-f9d544e22fb147fea36f99b4dcd77f50.jpg" alt="Leonardo-Pisano-Fibonacci-f9d544e22fb147fea36f99b4dcd77f50" border="0"></a>

## Using *Recursion* To Solve The Fibonacci Sequence Problem

    #include <bits/stdc++.h>
    using namespace std;
    
    int fibonacci(int x)
    {
    if (x <= 1)
    return n;
    return fibonacci(x - 1)+ fibonacci ( x - 2);
    }
    // check if the input number were 1 or 0, if not, we calculate the sum of the two numbers behind it in the series
          
    int main()
    {
    int x;
    cin >> x;
    cout << fibonacci(x);
    return 0;
    }
```
Time Complexity: O(2^n)
Space Complexity: O(n)
```

## Using *Binet’s formula* To Solve The Fibonacci Sequence Problem
In 1843, Binet gave a formula which is called “Binet formula” for the usual Fibonacci numbers by using the roots of the characteristic equation x 2 − x − 1 = 0


F_n	=	(phi^n-(-phi)^(-n))/(sqrt(5))	
	=	((1+sqrt(5))^n-(1-sqrt(5))^n)/(2^nsqrt(5))	
	

```
#include<iostream>
#include<cmath>

int fibonacci(int x) 
{
  float fai = (sqrt(5) + 1) / 2;
  return round(pow(fai, x) / sqrt(5));
}
 
int main ()
{
    int x;
    cin >> x; 
    cout << fibonacci(x); 
    return 0;
}

```

```
Time Complexity: O(log n) 
Space Complexity: O(1) 
```


|                |Time Complexity                          |Space Complexity                         |
|----------------|-------------------------------|-----------------------------|
|Recursion| O(2^n)            |O(n)            |
|Binet’s formula          |O(log n)            |O(1)            |
