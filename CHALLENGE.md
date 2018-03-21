![CF](https://camo.githubusercontent.com/70edab54bba80edb7493cad3135e9606781cbb6b/687474703a2f2f692e696d6775722e636f6d2f377635415363382e706e67) 29: Whiteboard Challenge
===

## Requirements

Create a function that accepts two arrays as it's input (represented as `arr1` and `arr2`).  Each array should contain a series of integers and the second array (`arr2`) should be a subset of the first array (`arr1`).  Your function should return a new array with all of the next greater numbers for `arr1` elements in the corresponding places of `arr2`.

The "next greater number" of a number `x` in `arr1` is the first greater number to it's right in `arr2`. If it does not exist, output `-1`. Otherwise, output the next greater number.

For example:

```javascript
// given
let arr1 = [4,1,2];
let arr2 = [1,3,4,2];

nextGreater(arr1, arr2)

// return
[-1,3,-1]
```

## Submission Instructions

1. With your assigned partner, pseudocode your solution on the whiteboard. Take a picture of your proposed solution for your repo.
1. Make a new branch and folder in your whiteboard challenge repository on GitHub. The name of the folder should be the same as the name of the challenge.
1. This folder should contain:
  - A file named `solution.js` which contains the JavaScript solution
  - A `__test__` directory that includes your `solution.test.js` file and associated tests
  - A picture of your pseudocoded solution from the whiteboarding exercise
  - A `README.md` which includes the problem domain
1. Complete the whiteboard challenge in your text editor, and verify that it's functional
1. Make a pull request from your working branch to your master branch
1. Submit a link to your PR on Canvas or submit a link to your `repo/daily-whiteboarding-directory/solution.js`