1. What will happen at line 12 and why? If the code causes an error, explain why.
   3
2. What will happen at line 13 and why? If the code causes an error, explain why.
   150
3. What will happen at line 14 and why? If the code causes an error, explain why.
   150
4. What will this function return? Give a brief explanation why. If the code causes an error, explain why.
   This function returns [50, 100, 150] because it applies a 50% discount to each item in the input array [100, 200, 300]. Inside the loop, each discounted price is calculated by multiplying the original price by (1 - discount), which equals 0.5. The result is then rounded to two decimal places using Math.round(... * 100) / 100 and added to the discounted array. 
5. What will happen at line 12 and why?  If the code causes an error, explain why. (assume this function is being called like the others: discountPrices([100, 200, 300], 0.5)).
   This will throw an error because the code is trying to access i outside the for loop and i is defined as let, so i is not defined.
6. What will happen at line 13 and why? If the code causes an error, explain why. 
   This will throw an error because the code is trying to access discountedPrice outside the for loop, and discountedPrice is defined as let, so discountedPrice is not defined.
7. What will happen at line 14 and why? If the code causes an error, explain why.
   150
8. What will this function return? Give a brief explanation. If the code causes an error, explain why.
   This function returns [50, 100, 150] because it applies a 50% discount to each item in the input array [100, 200, 300]. Inside the loop, each discounted price is calculated by multiplying the original price by (1 - discount), which equals 0.5. The result is then rounded to two decimal places using Math.round(... * 100) / 100 and added to the discounted array.
9.  What will happen at line 11 and why? If the code causes an error, explain why.
    This will throw an error because the code is trying to access i outside the for loop and i is defined as let, so i is not defined.
10. What will happen at line 12 and why? If the code causes an error, explain why.
    3
11. What will this function return? Give a brief explanation. If the code causes an error, explain why.
    This function returns [50, 100, 150] because it applies a 50% discount to each price in the input array [100, 200, 300]. It calculates each discounted price by multiplying the original price by (1 - discount), which is 0.5, and stores the results in a new array. The loop runs correctly, and all variables are scoped properly using let and const. 
12. Given the above Object, write the notation for:
    Accessing the value of the name property in the student object
    student.name
    Accessing the value of the Grad Year property in the student object
    student["Grad Year"]
    Calling the function for the greeting property in the student object
    student.greeting()
    Accessing the name property of the object in the Favorite Teacher property in student
    student["Favorite Teacher"].name
    Access index zero in the array of the courseLoad property of the student object
    student.courseLoad[0]
13. Arithmetic
    A. '3' + 2
    '32' The + operator performs string concatenation when one operand is a string. Here, '3' is a string, so 2 is converted to a string ('2') and concatenated, resulting in '32'.
    B. '3' - 2
    1 The - operator in JavaScript performs numeric subtraction and attempts to convert operands to numbers. '3' is converted to the number 3, and 3 - 2 equals 1.
    C. 3 + null
    3 In numeric operations, null is converted to 0. So, 3 + null becomes 3 + 0, which equals 3.
    D. '3' + null
    '3null' The + operator performs string concatenation because '3' is a string. null is converted to the string 'null', so '3' + 'null' results in '3null'.
    E. true + 3
    4 In numeric operations, true is converted to 1. So, true + 3 becomes 1 + 3, which equals 4.
    F. false + null
    0 In numeric operations, false is converted to 0, and null is converted to 0. So, false + null becomes 0 + 0, which equals 0.
    G. '3' + undefined
    '3undefined' The + operator performs string concatenation since '3' is a string. undefined is converted to the string 'undefined', so '3' + 'undefined' results in '3undefined'.
    H. '3' - undefined
    NaN The - operator attempts to perform numeric subtraction. '3' is converted to the number 3, but undefined converts to NaNin numeric contexts. Any operation involving NaN results in NaN.
14. Comparison
    A. '2' > 1 true. In comparisons, JavaScript converts operands to numbers if one is a number. '2' is converted to 2, so 2 > 1 is true.
    B. '2' < '12' false. When comparing two strings, JavaScript performs lexicographical comparison. '2'  is greater than '12', so '2' < '12' is false.
    C. 2 == '2' true. The == operator performs loose equality with type coercion. '2' is converted to the number 2, so 2 == 2 is true.
    D. 2 === '2' false. The === operator checks strict equality without type coercion. 2 (number) and '2' (string) have different types, so 2 === '2' is false.
    E. true == 2 false. The == operator performs type coercion. true is converted to 1 in numeric contexts, so true == 2 becomes 1 == 2, which is false.
    F. true === Boolean(2) true. Boolean(2) converts the number 2 to a boolean. Any non-zero number is true, so Boolean(2) is true. The === operator checks strict equality, and both true and Boolean(2) are booleans with the value true, so true === Boolean(2) is true.
15. Explain the difference between the == and === operators.
    In JavaScript, the == operator compares two values for equality after converting them to the same type through type coercion. On the other hand, the === operator compares both the value and the type without any type coercion.
16. Given the above Object, write a for...in loop that will iterate through it and print out the value of
    the property if the property starts with the letter r, or if the value of that property is an odd number.  (This should be in a JS file part2-question16.js)
17. If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what
    will be the result? Briefly walk through how you arrived at that result. (This should be in your part2.md). Here we are passing in a function as a parameter, however we can also return a function from another function just as easily, you're encouraged to play around with callbacks as they are used heavily in frontend JS development. 
    The result will be [2, 4, 6]. When modifyArray([1, 2, 3], doSomething) is called, the modifyArray function starts by creating an empty array newArr. It then loops through the input array [1, 2, 3], applying the doSomething callback to each element, which doubles the number. In the first iteration, doSomething(1) returns 2, which is pushed to newArr, making it [2]. In the second iteration, doSomething(2) returns 4, updating newArr to [2, 4], and in the third iteration, doSomething(3) returns 6, resulting in newArr as [2, 4, 6]. Finally, modifyArray returns newArr, so the result of the function call is [2, 4, 6]. This process demonstrates how the callback function doSomething transforms each element of the array by doubling it.
18. The above program only prints out the time once when executed. Modify this code such that the program
    prints out the current time every second.  (This should be a JS file - part2-question18.js)
19. What is the output of the above code? (This should be in your part2.md)
    1
    4
    3
    2