1. At line 12 the code will print ```3```. The for-loop stops iterating when the value of the variable ```i``` equals the length of the array stored in the variable prices, which is of length 3. Since the variable ```i``` is of type var, it's value's scope is the entire function.
2. At line 13 the code will print ```150```. Since the variable ```discountedPrice``` is of type var, then its scope is the entire function. Therefore, in line 13 it outputs the last stored value (prices[2] * (1-0.5) <-> 300*0.5 <-> 150.
3. At line 14 the code will print ```150```. Since the variable ```finalPrice``` is of type var, then its scope is the entire function. Similarly as above, at line 14 ```finalPrice``` outputs the last stored value which is the same value as ```discountedPrice``` as explained in Question 2.
4. The function will return the array ```[50,100,150]```. This is because the for-loop iterates through the values of the ```prices``` array and applies a discount to each value. At each iteration, once the final price is calculated and stored in the variable ```finalPrice```, the value stored in ```finalPrice``` is pushed into the array stored in the variable ```discounted```. Since ```discounted``` is of type var, its scope is the entire function.
5. The code will return an error at line 12 since it is trying to access the variable ```i``` which is out of scope. Since ```i``` is of type ```let``` and is declared within a for-loop, its scope is only within the for-loop block.
6. The code will return an error at line 13 because it is trying to access the variable ```discountedPrice``` which is out of scope. Since ```discountedPrice``` is of type ```let``` and is declared within a for-loop, its scope is only within the for-loop block.
7. The same thing will occur as in question 3. Although now the variable ```finalPrice``` is of type ```let```, it has a function-scope and its behavior is not changed.
8. The same thing will occur as in question 4. Although now the variable ```discounted``` is of type ```let```, it has a function-scope and its behavior is not changed.
9. The code will return an error at line 11 because it is trying to access the variable ```i``` which is out of scope. Since ```i``` is of type ```let``` and is declared within a for-loop, its scope is only within that for-loop.
10. At line 12 the code will print ```3```, which is the length of the array stored in the variable ```prices```. Since the variable ```length``` is of type const, it has a function-scope.
11. The code will return ```[50,100,150]```. Since there are no references to variables out of the function-scope, the code does not return any errors.
12. a. ```student.name```
    b. ```student['Grad Year']```
    c. ```student.greeting()```
    d. ```student['Favorite Teacher'].name```
    e. ```student.courseLoad[0]```
13. a. In the expression ``` '3' + 2 ```, the integer ```2``` is mapped to its string representation. Therefore the output is ```'35'```
    b. In the expression ```'3'-2```, the string ```'3'``` is mapped to its integer representation. Therefore the output is ```1```.
    c. In the expression ```3 + null```, the value ```null``` is mapped to its integer representation ```0```. Therefore the output is ```3```.
    d. In the expression ```'3'+ null```, the value of ```null``` is mapped to its string representation. Therefore the output is ```'3null'```.
    e. In the expression ```true + 3```, the value of ```true``` is mapped to its integer representation. Therefore the output is ```4```.
    f. In the expression ```false + null```, both ```false``` and ```null``` are mapped to their integer representations. Therefore the output is ```0```.
    g. In the expression ```'3' + undefined```, the value of ```undefined``` is mapped to its string representation. Therefore the output is ```3undefined```.
    h. In the expression ```'3' - undefined```, both ```'3'``` and ```undefined``` are mapped to their integer representations. Since the mapping of ```undefined``` is ```NaN```, the ouput is ```NaN```.
14. a. In the expression ```'2'>1```, the value of ```'2'``` is mapped to its integer representation. Therefore the output is ```true```.
    b. In the expression ```'2'<'12'```, the strings are compared character by character. Therefore it compares ```'2'<'1'``` and outputs false.
    c. In the expression ```2 == '2'```, the value of ```'2'``` is mapped to its integer representation. Therefore, the output is ```true```.
    d. In the expression ```2 === '2'```, the strict equality operator checks if the two values are of the same type. Therefore, the output is ```false```.
    e. In the expression ```true == 2```, the value of ```true``` is mapped to its integer representation ```1```. Therefore, the output is ```false```.
    f. In the expression ```true === Boolean(2)```, the value of ```Boolean(2)``` is mapped to its boolean representation ```true```. Therefore, the output is ```true```.
15. The ```==``` operator checks for equality between the value on the left hand side and right hand side. If the operands are of different types then they are mapped to their integer representations. On the other hand, the ```===``` operator does not do type conversion. Instead, it only checks if the operands are of the same type.
17. At line 13, two parameters are been passed into the function ```modifyArray(array,callback)```. ```array``` stores the value ```[1,2,3]``` and variable ```callback``` stores the function ```doSomething```. Inside of ```modifyArray```, first we create an empty array ```newArr```. Then the for-loop iterates 3 times (the length of ```array```) and makes a call to the function stored in ```callback``` which is ```doSomething``` with an input of the i-th value of ```array```. Inside of ```doSomething```, the passed in parameter is doubled and is returned. Therefore back on line 4, the value returned from ```doSomething``` is pushed into the array ```newArr```. Finally, ```modifyArray``` returns ```newArr``` with the value ```[2,4,6]```.
18. 