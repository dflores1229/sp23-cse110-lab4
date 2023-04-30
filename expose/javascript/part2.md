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