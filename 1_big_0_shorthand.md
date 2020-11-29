1. Arithmetic operations are constant
adding, subtracting, dividing is a constant.

2+2 and 100000 + 2 are same

2. Variable assignment is constant.
x = 1000 is same as x = 10000000  

3. Accessing elements in an array (by index) or object (by kay) is also constant

4. In a loop, the complexity is the length of the loop times the complexity of whatever happens inside of the loop.

The best case scenario is that it will run 5. But it does not matter to us. We care about n growing to numbers of milions. And this depends on the length of the array.
Therefor it is O(n);

```javascript
    const logAtLeast5(n) {
        for (var i = 1; i <= Math.max(5, n); i ++){
            console.log(i);
        }
    }
```


It will run most 5 times.
It is O(1). Simplified for O(5)

```javascript
    const logAtMost5(n) {
        for (var i = 1; i <= Math.min(5, n); i ++){
            console.log(i);
        }
    }
```

