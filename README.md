# React Calculator

For this assignment, your task is to build a React calculator application that performs basic arithmetic. Start by forking and cloning this repository to your development environment. Then, using the provided [template files](template) and _without_ using the `eval()` function, create a React calculator application that performs multiplication.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/327/09CFCA62-18ED-4099-8729-65BFC9FA06AC-570-0000E58832829D6F.gif)

Performs division.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/328/A30388D2-BB83-4A8F-9E76-97DDAF96ADF4-570-0000E5B36DF6C262.gif)

Performs addition.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/329/0BC48E07-DE52-4BDA-8E20-8D97C3307EE3-570-0000E5E1BFC8C414.gif)

And performs subtraction.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/330/DE496CDB-FC2A-4B80-AC1F-EB2332A92CA8-570-0000E605156A0BC0.gif)

The calculator must work with both positive and negative operands.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/331/A1968884-C505-4E0B-910D-227916951B5D-570-0000E640707F5D21.gif)

And the clear button must delete the contents of the screen.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/334/1885D50C-8FD7-43EE-828B-B83B557F4A87-570-0000E750F29CABD4.gif)

If the arithmetic expression is not valid, the screen must display the word `Error` and all operand, operator, and equal button clicks are ignored until the clear button is clicked.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/333/5DA284D3-0324-47C2-838D-DDF48B977DAF-570-0000E71FA1DC32CC.gif)

Likewise, if the arithmetic expression contains more than one operator, the screen must display the word `Error` and all operand, operator, and equal button clicks are ignored until the clear button is clicked.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/332/4D915844-BA7F-4C9C-AD8F-A84D38CD43B9-570-0000E6DBC3243DBB.gif)

**HINT #1:** Display a blank screen when the application first renders.

**HINT #2:** When evaluating the screen's arithmetic expression, [match](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/match) it with the following regular expression.

```js
/^(\-?\d+)(x|\/|\+|\-)(\-?\d+)$/
```

For example, matching the arithmetic expression `-1+2` to the above regular expression works like this.

```js
const matches = '-1+2'.match(/^(\-?\d+)(x|\/|\+|\-)(\-?\d+)$/);
console.log(matches);  // ["-1+2", "-1", "+", "2"]
```

The `String.prototype.match()` function returns `null` if there's no match. In this case, update the screen with the word `Error`. However, if there's a match, evaluate the arithmetic without using the `eval()` function and update the screen with its results.

**HINT #3:** Figure out how to map the plus `"+"` string to the actual JavaScript plus `+` operator. Once you figure that out, apply the same technique to the other arithmetic operators.

## Bonus

Refactor the application to handle keyboard input to the calculator's screen. When the screen is focused, input from the keyboard must must change the screen's value.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/335/6C6C95A9-8085-49D9-B5B7-9554DF4EA3D6-570-0000E8D7D15F6298.gif)

Pressing the `Enter` key must evaluate the screen's arithmetic expression.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/336/6EF631C7-5319-4C59-A49A-7621A612EA2F-570-0000E91BAEA524F4.gif)

And pressing the `Escape` key must clear the screen.

![](https://students-gschool-production.s3.amazonaws.com/uploads/asset/file/337/FBA76FD0-D9AA-4B3E-8056-EDFBA8FA581D-570-0000E92E7FDEB483.gif)

## Bonus

Using your preferred ESLint rules, lint your project with the `npm run lint .` command.

## Bonus

Refactor the application to correctly handle arithmetic expressions that contain more than one operator.

## Bonus

Once you're satisfied, find a classmate and see if that person would like some help.

## Solution

The [solution](https://github.com/gSchool/wd-react-calculator-solution) is available to instructors as well as students who've completed this assignment.
