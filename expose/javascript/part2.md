1. It will print 3. Because i was declared using ``var``, it is function-scoped. This means it is still accessible outside of the for loop. The loop iterates for indices 0, 1, and 2. It increments to 3, the condition 3 < 3 fails, the loop terminates, and 3 is printed.

2. It will print 150. ``discountedPrice`` is declared with ``var``, so it can be accessed outside the for loop. It saves the last iteration of the loop, which is 300 * (1 - 0.5) = 150.

3. It will print 150. ``finalPrice`` was defined with ``var`` at line 4, so it is accsessible. Its final value is updated in the last loop iteration to 150.

4. It will return the array [50, 100, 150]. The function works through the array and applied a 50% discount to each item, rounds the result, and pushes it into the ``discounted`` array. 

5. It will cause a error, because the variable ``i`` is initialized with ``let`` inside the for loop, and since let is not  visible through blocks, so ``i`` is only accessible inside the loop.

6. It will cause a error, as ``discountedPrice`` is declared using ``let`` inside the for loop block, and is not visible outside the block.
   
7. It will print 150, because ``finalPrice`` was initialized using let on line 4, and it is inside the main function block, and line 14 is also in the main function block. This means that it has access to the variable.

8. It will return the array [50, 100, 150]. As the function still works perfectly fine using ``let`` instead of ``var``. Similar to question #4, the function works and applies a 50% discount to each item and into the ``discounted`` array.

9.  It will cause a error. Just like in #5, ``i`` is declared using ``let`` inside the for loop. This makes it so that its unable to be accessed outside of loop.
    
10.  It will print 3, because ``length`` is declared with ``const`` at line 4, with ``prices.length``, which is 3. Because line 12 is in the same block function as line 4, it will sucessfully print 3.

11. The function will return the array [50, 100, 150]. The function works like normal and returns the 50% off version. This works even though its a ``const`` because the contents of the array are mutable using .push, and the ``const`` in the loop is fine aswell, because each iteration a new ``discountedPrice`` is created.

12. 
    A. student.name
    B. student['Grad Year']
    C. student.greeting()
    D. student['Favorite Teacher'].name
    E. student.courseLoad[0]

13. 
    A. ``'32'`` - JS can see string and number with the ``+`` operator, so it converts the number to the string and strings it together.  \
    B. ``1`` - The ``-`` operator only works with numbers, so JS converts the string iinto the number 3. \
    C. ``3`` - ``null`` is converted to 0 when performing addition with a number. \
    D. ``3null`` - ``null`` is converted to string ``"null"`` to string it together. \
    E. ``4`` - ``true`` is converted to number 1, and does addition. \
    F. ``0`` - ``false`` is converted to 0, and ``null`` is 0. \
    G. ``3undefined`` - ``undefined`` becomes a string to string it together. \
    H. ``NaN`` - Because it subtracted ``undefined`` which results in NaN. 

14. 
    A. ``true`` -  The string is converted to number and 2 > 1. \
    B. ``false`` - Both are strings so JS compares the two alphabetically, and since '2' is greather than '1' it returns false. \
    C. ``true`` - SInce its two equal signs, it checks for equality with type conversion. \
    D. ``false`` - Because it has three equal signs, it checks the equality without type conversion. \
    E. ``false`` - True converts to 1, and 1 is not equal to 2. \
    F. ``true`` - Any non zero number convertd to a boolean is true, so true === true. 

15. The difference between ``==`` and ``===`` is that ``==`` performs a comparison with type conversion before comparing the values, while the ``===`` operator performas a equality check without converting the type. 

16. part2-question16.js 

17. result: ``[2, 4, 6]``
    Function modifyArray is called with array ``[1, 2, 3]``, and function doSomething. Inside the for loop, it iterates through the array, and for each element it calls ``callback`` which is the function ``doSomething``. ``doSomething(1)`` returns 2, and is pushed into ``newArr``, and ``doSomething(2)`` retunrs 4, and ``doSomething(3)`` returns 6, which is all pushed into ``newArr``. This creates the returning array of ``[2, 4, 6]``. 

18. part2-question18.js
19.  Output:
````
1
4
3
2
````
