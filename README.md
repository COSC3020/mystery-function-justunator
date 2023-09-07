[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11754407&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0]; //this checks of a only has 1 element in the array and returns the element if true
    var foo = mystery(a.slice(1, a.length)) //this creates var foo with 1 element from the array. The main checking happens during this recursion.
    if(foo > a[0]) return foo; // compares foo with the first element in a to see if foo is larger
    else return a[0]; //returns a[0] if foo isnt larger, but returns foo when foo is larger
    //this function returns the maximum value from an array
}
```
