We can use big O notation for space complexity.
as n grows.

As n gorws, size of input grows (we ignore this part.)
it is called Auxiliary space complexity to refer to space required by the algorithm, not including space taken up by the inputs.

# Main rules:

- most primitives (booleans, numbers, undefined, null) are constant space. boolean = 1000

- strings are difrent. They require O(n) where n is the string length (i.e 1 char string and 50 char string)

- arrays and objects are same as strings as their complexity grows as their length grows.

Space complexity bigO  of the array is O(2) so in shorthand it is O(1)

```javascript
const sum = (arr) => {
    // we got one variable called total
    let total = 0;
    //  we got another variable in the loop
    for(let i = 0; i < arr.length; i++){
        total += arr[i];
    }

    return total;
}
```


```javascript
    const double = arr => {
        // 1 array
        let newArr = [];
        // 1 variable
        for(let i = 0; i < arr.length; i++){
            newArr.push(2 * arr[i]);
        }
        return newArr;
        // O(n + 1) shortened to O(n)
    }

```