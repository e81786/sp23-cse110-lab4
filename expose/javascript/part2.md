# Part 2

1. It prints `3`, because when it loops through the for loop, it goes through the prices of `[100, 200, 300]`, updating `i` in each iteration. As it finishes looping through `prices.length`, the for loop stops when `i` is greater than or equal to `prices.length`, thus it stops at `i = 3` because `prices.length` is `3`. Thus, line 12 prints `3`.
2. It prints `150`, because the at the end of the for loop, `discountedPrice` is equal to `prices[2] * (1 - discount)`, which is equal to `300 * (1 - 0.5)` which is `150`. Thus, line 13 prints `150`.
3. It prints `150`, because at the end of the for loop, `finalPrice` is equal to `Math.round(discountedPrice * 100) / 100`, which is then equal to `Math.round(150 * 100 / 100)`, which is `150`. Thus, line 14 prints `150`.
4. This function returns `[50, 100, 150]`, because the for loop goes through the inputted `prices` and it multiplies it by the inputted `discount`, then it rounds it, then it pushes it to the `discounted` array that holds all the discounted prices. Thus, it applies a `50%` discount to each inputted price. As the prices inputted are `100, 200, 300`, the final discounted prices come out to be `50, 100, 150`, and the array is returned by the function.
5. The code causes an error because it is attempting to print `i`, which is a `let` variable only within the scope of the `for` loop, thus `i` doesn't exist outside of the for loop, causing an error.
6. The code causes an error because it is attempting to print `discountedPrice` which was intialized within the scope of the `for` loop, and it cannot print the `let` variable outside the `for` loop, thus it causes an error.
7. It prints `150`, this is for the same reasons as #3, but also does not create an error because it is created before the `for` loop using `let`, thus allowing it to be used throughout the entire function, and thus it can be accessed by `console.log` in line 14.
8. This function returns `[50, 100, 150]` for the same reasons as #4 and #7. It runs through the code, changing each price in `prices` to the discounted price, and the `let` keyword allows it to be accessed in the scope of the entire function.
9. It returns an error for the same reason as #5, it is trying to access `i` outside of its scope of the `for` loop.
10. It prints `3` because line 12 prints `length` which is a `const` variable that is declared at the very beginning and never changed, thus `length` always stays as the `prices.length` which is 3.
11. This function will return `[50, 100, 150]`, which is what it returns as in #4 and #8, because the it does what it was set out to do, change all the `prices` into the discounted prices. It works because all the `const` variables are used within their proper scope, and they are not changed any point, so they are used properly and the proper response of `[50, 100, 150]` is returned.
12. a. student.name
    b. student['Grad Year']
    c. student.greeting()
    d. student['Favorite Teacher'].name
    e. student.courseLoad[0]
13. a. `32`, because `'3'` is a string, so javascript just concatenates 2 onto `'3'` as if it is also a string, also because the `+` operator is used for concatenation.
    b. `1`, as the `-` operator cannot be used with strings, so Javascript assumes that they are now both numbers, converting `'3'` to 3, and then subtracting 2 from it.
    c. `3`, because using the `+` operator with `null` and an int converts `null` to an integer of 0.
    d. `3null`, because when adding a string using `+`, null is then also converted to a string to concatenate onto 3.
    e. `4`, because `true` maps to 1, especially when dealing with ints.
    f. `0`, because we are not dealing with strings, thus js uses numeric conversion, and both `false` and `null` both map to 0.
    g. `3undefined`, because `'3'` is a string, it then converts `undefined` to a string and concatenates it.
    h. `NaN`, because the `-` operator only allows for Numeric conversion, but converting `undefined` to numerics just gives `NaN`.
14. a. `true`, because when comparing a numeric string to an int, the string `'2'` becomes 2, which is greater than 1.
    b. `false`, because when both in the comparison are strings, the comparison goes in lexicographical order starting from the first character, thus `'1'` is less than `'2'`, making it false.
    c. `true`, again, when comparing numeric string to an int, the string `'2'` becomes 2, which is the same as 2.
    d. `false`, because the types do not match and the `===` operator compares without type conversion, they are not the same.
    e. `false`, because when doing comparison with booleans and ints, `true` maps to 1, which is not equal to 2.
    f. `true`, because typecasting 2 using `Boolean(2)` makes it `true`, as any value that are not empty values are `true` when converting to Boolean; thus when comparing `true` to `Boolean(2)`, even the `===` operator recognizes that they are equal.
15. The `==` operator checks for equality, but also does type conversion, thus changing the values to match properly; however the `===` operator checks for equality without type conversion, thus checking if both type and value match.
16. See [part2-question16.js](/expose/javascript/part2-question16.js)
17. The result would be `[2, 4, 6]`. I got to this conclusion because `modifyArray` is passed the values `[1, 2, 3]` and `doSomething`. `modifyArray` then for loops through the arrays length, in this case `3`, and it pushes a new value into the `const` array `newArr`. This value that is being pushed back is one that is returned from a callback to a different function that was passed in, `doSomething`, passing each of the original array's values. `doSomething` then multiplies the values by 2, and returns it to be pushed back into `newArr`. At the end, `newArr` is returned, giving us the same size array that was passed in, just with all the numbers doubled.
18. See [part2-question18.js](/expose/javascript/part2-question18.js)
19. `1 4 3 2`
