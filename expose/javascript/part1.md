1. It will print: ``values added: 20``. Because ``add`` is true, and sets variable ``result`` is set to 0, and then reset to the sum of ``num1`` and ``num2``, which is 10+10=20. 
2. It will print: ``final result: 20``. Because ``var`` is function-scpoed, so they are visible through blocks (inside the sumValues function), even though its outside the if function where it was initially declared. 
3. You should not use ``var`` because it is visible through blocks, this can be hard to track the variables and could create conflicts though the code, as it will be available to the **whole** function.


4. It will print ``values added: 20``. The logic inside the if block works perfectly fine, so the result of the two numbers added will work perfectly fine.
5. The code will return an error, because ``result`` will not be defined in line 13, as the variable will not exist after the if block statement, since ``let`` is not visible though blocks. 


6. This code will return an error, as in line 7, since ``result`` was declared using ``const``, it cannot be reassigned after it was initially declared. 

7. The code will return an error since similar to ``let``, ``const`` cannot be accessed outside the if block it was declared in.