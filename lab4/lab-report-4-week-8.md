__CSE 15L Lab Report-4-week8__
=========
## Ziyou Zhao ziz021@ucsd.edu

***
## _**Links**_

[Link to my Repository](https://github.com/Jameszzyyyyy/markdown-parse)

[Link to Repository I reviewed](https://github.com/AchuthKrishna/markdown-parse)

## _**Snippet1**_

_**Preview:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet1-preview.png?raw=true)

_**Code for Junit Test:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet1-test.png?raw=true)

_**My Output**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet1-my-output.png?raw=true)

_**Reviewed Output**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet1-reviewed-output.png?raw=true)

_**Code Change**_

I believe that a small change would be able to fix the problem in my program. The problem now is that it count `url.com` as a valid link while count `ucsd.edu` as an invalid one. For `url.com`, I only need a `if statement` to check if the openbracket is at the first index; and for `ucsd.edu`, it causes error because of the nested bracket, I think I only need a `if statement` to check if the previous character is at backtick.


## _**Snippet2**_

_**Preview:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet2-preview.png?raw=true)

_**Code for Junit Test:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet2-test.png?raw=true)

_**My Output**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet2-my-output.png?raw=true)

_**Reviewed Output**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet2-reviewed-output.png?raw=true)

_**Code Change**_

I believe that a small change of code will not able to fix the problem, the problem now is that the index is out-of-bound. In order to fix it, I will have to check many different things to make it be able to pass in different situations, such as check if there is additional brackets. These changes will be more than 10 lines.


## _**Snippet3**_

_**Preview:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet3-preview.png?raw=true)

_**Code for Junit Test:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet3-Test.png?raw=true)

_**My Output**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet3-my-output.png?raw=true)

_**Reviewed Output**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab4/report4-snippet3-reviewed-Output.png?raw=true)

_**Code Change**_

Similar to Snippet2, I don't think that a small change will be able to fix the problem I have now, the problem is also index-out-of bound, and I will have to check if there is a missing `openbracket`, `closeparen`, these changes may take more than 10 lines.
