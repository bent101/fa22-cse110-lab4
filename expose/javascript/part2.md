# Part 2

1. 3 will be printed, because the `for` loop will terminate when `i < prices.length` is true. Since `i` starts at 0 and is incremented one at a time (`i++`), this will happen when `i === prices.length`. In our case, `prices.length` is 3, so `i` will be 3 on line 12. `i` will still be accessible on line 12 because it was declared with `var`, so it has function scope.
2. 150 will be printed, because `discountedPrice` will be the last value it was assigned to in the `for` loop. In our case, that's `prices[2] * (1 - 0.5)` = `300 * 0.5` = `150`.
3. 150 will be printed again, because `finalPrice` will also be the last value it was assigned to, which is `Math.round(discountedPrice * 100) / 100` = 150.
4. `[50, 100, 150]`. It essentially multuplies the `prices` array by `1 - discount` and rounds the results to the nearest cent. In our case, `[100, 200, 300] * 0.5 = [50, 100, 150]`.
5. Since `i` was declared with `let` this time, it will be out of scope at line 12, so we will get an error saying `i` wasn't defined.
6. Same as above
7. 150 will be printed, since `finalPrice` was declared on line 4 outside of the `for` loop, so it is still in scope at line 14.
8. `[50, 100, 150]`, same as #4
9. We will get an error. `i` will be out of scope at line 11 since it was declared with `let`.
10. 3 will be printed, because `length` was defined as `prices.length` (which is 3 in our case) on line 4, so it is in scope on line 12.
11. `[50, 100, 150]`, same as #4 and #8
12. a. `student.name` \
b. `student['Grad Year']` \
c. `student.greeting()` \
d. `student['Favorite Teacher'].name` \
e. `student.courseLoad[0]`

13. a. `'32'`, beacuse `2` is converted to `'2'` \
b. `1`, because `'3'` is converted to `3` \
c. `3`, because `null` is converted to `0` \
d. `'3null'`, because `null` is converted to `'null'` this time, because `'3'` is a string now instead of a number \
e. `4`, because `true` is converted to `1` \
f. `0`, because `false` and `null` are both converted to `0` so they can be added \
g. `'3undefined'`, because `undefined` is converted to `'undefined'`  \
h. `NaN`, because while `null` converts to the number `0`, `undefined` converts to the "number" `NaN`.

14. a. `true`, because '2' is converted to `2` \
b. `false`, becaues `'12'` comes before `'2'` alphabetically \
c. `true`, because `'2'` is converted to `2` \
d. `false`, because `===` doesn't do any type converting \
e. `false`, because `true` converts to `1` \
f. `true`, because `Boolean(2)` evaluates to `true`, and `true === true` \

15. `==` uses type conversion to try to "make things work"; `===` doesn't
16. [see code](/expose/javascript/part2-question16.js)
17. `modifyArray` essentially returns `array`, but with `callback` applied to each element. `doSomething` doubles a number, so `modifyArray([1, 2, 3], doSomething)` returns `[2, 4, 6]`.
18. [see code](/expose/javascript/part2-question18.js)
19. Output:

```
1
4
3
2
```
