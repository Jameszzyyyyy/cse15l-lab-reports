__CSE 15L Lab Report-5-week10__
=========
## Ziyou Zhao ziz021@ucsd.edu

***

## _**194.md**_

Instead of using `diff`, I manually run the test file `194.md` on my implementation and class implementation separately, and compare their results.

- **Different Results**

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab5/194test.png?raw=true)

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab5/194.png?raw=true)

- **Which one is correct & How to fix**

Between these two results, I would say that mine is more likely to be the correct one because there are `:` and texts outside the parentheses and behind the `closeBracket` in the test file `194.md`, the link is not valid. Therefore, we should add some codes to check if there is text between `closeBracket` and `openParen`, and see if `openParen` is right after the `closeBracket`.

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab5/194fix.png?raw=true)


## _**510.md**_

- **Different Results**

Same as the `194.md`, I manually run `510.md` on both implementations separately and compare their ourputs

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab5/510test.png?raw=true)

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab5/510.png?raw=true)

- **Which one is correct & How to fix**
Again, I think that my implementation is correct while the one I cloned is incorrect because there is a space between the `closeBracket` and the `openParen`. So that the cloned implemantation with the result of `[/url]` should print nothing. In order to fix it, similar to how to fix the code for `194.md`, we should add a `if` statement to see if there is space between `openParen` and `closeBracket`, which means whether the `openParen` is right after `closeBracket`.

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab5/510fix.png?raw=true)