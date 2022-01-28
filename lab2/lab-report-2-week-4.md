__CSE 15L Lab Report-2-week4__
=========
## Ziyou Zhao ziz021@ucsd.edu

***
## _**First Code Change**_

_**Code:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab2/lab2-1changes.png?raw=true)

_**Link to the file:**_

[test-file2](https://github.com/Jameszzyyyyy/markdown-parse/blob/main/test-file2.md)
(missing close parentheses)

_**Symptom:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab2/lab2-1output.png?raw=true)

_**Description:**_

This bug appears because there is no close parentheses can be found in the file, so that when we compile and run the code, it shows in terminal that `StringIndexOutOfBoundsException`. Therefore, everythime when we write the code, we should try to consider very extreme cases about index.

***
## _**Second Code Change**_

_**Code:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab2/lab2-2changes.png?raw=true)

_**Link to the file:**_

[test-file3](https://github.com/Jameszzyyyyy/markdown-parse/blob/main/test-file3.md)
(having two open parentheses)

_**Symptom:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab2/lab2-2output.png?raw=true)

_**Description:**_

This happens when we have two open parentheses, the code will include the second one into the result and print it out. So that when we see this kind of problem, we need to consider it as a possible case and find the solution to remove it from the result.

***
## _**Third Code Change**_

_**Code:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab2/lab2-3changes.png?raw=true)

_**Link to the file:**_

[test-file2](https://github.com/Jameszzyyyyy/markdown-parse/blob/main/test-file2.md)
(should print nothing but "[]')

_**Symptom:**_

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab2/lab2-3output.png?raw=true)

_**Description:**_

When I run the code in tester, it should a bug which says the test case expect to have a result as `java.util.ArrayList<[]>`, but the value I set for `expect` was `java.util.ImmutableCollections$List12<[]>`, this symptom shows that every time when we set the case in tester, we should consider the type of value carefully, otherwise a bug may appear.
