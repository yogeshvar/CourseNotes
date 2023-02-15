## TDD 

```java
Public double x ( double y ) { 
	double z = getB();
	z = z - y;
	return z;
}
```


| Y  	| getB() 	| Actual  	| Expected 	|
|----	|--------	|---------	|----------	|
| 5  	| 6      	| 1       	| 1        	|
| -5 	| 6      	| 11      	| 11       	|

Real world example:

```java
Public double deposit( double salary ) { 
	double balance = getBalance();
	balance = balance - salary;
	return balance;
} 
```