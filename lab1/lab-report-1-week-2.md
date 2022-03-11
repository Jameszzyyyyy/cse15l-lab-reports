__CSE 15L Lab Report-1-week2__
=========
## Ziyou Zhao ziz021@ucsd.edu

***
## __Installing VScode__

- Go to the VSCode website https://code.visualstudio.com.
- Follow the instructions to download the correct version for your operating system.


![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab1-VSCode.png?raw=true)

***
## __Remotely Connecting__

- Go to https://sdacs.ucsd.edu/~icc/index.php and find your acount.
- Go to VSCode and open the Terminal.
- Enter `ssh cs15lwi22***@ieng6.ucsd.edu` where *** is different for everyone.
- Enter the password, reset if it doesn't work.


![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab1-Remotely%20Connecting.png?raw=true)

***
## __Trying Some Commands__

_Try some commands such as `cd`, `ls`, `pwd`_

- `cd`  stands for change directory, for example: `cd cse15l` means change to directory cse15l.
- `ls` stands for list, it will list all files under the current directory.
- `pwd` will show the path of the current directory.


![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab1-Trying%20Some%20Commands.png?raw=true)

***
## __Moving Files with `scp`__

- Create a file on your computer called WhereAmI.java with the following content:

```
class WhereAmI {
    public static void main(String[] args) {
        System.out.println(System.getProperty("os.name"));    
        System.out.println(System.getProperty("user.name"));
        System.out.println(System.getProperty("user.home"));
        System.out.println(System.getProperty("user.dir"));
    }
}
```
- Use the command `scp WhereAmI.java cs15lwi22***@ieng6.ucsd.edu`, so that we can move the file to the server.

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab1-Moving%20Files%20with%20scp.png?raw=true)

***
## __Setting an SSH Key__

- Run the code `ssh -keygen` and create a pair of files called the _public key_ and _private key_.
- After enter the file and passphrase, you will receive a random image like:

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab1-Setting%20an%20SSH%20Key.png?raw=true)
- You will now be able to see two new files on your system.
- Copy the public key to the .ssh directory of your user account on the server
use `ssh` command again.
- Then enter `mkdir .ssh`, `<logout>` and `scp /User/***/.ssh/id_rsa.pub cs15lwi22@ieng6.ucsd.edu:~/.ssh/authorized_keys`.
- After doing all these, you don't need to type your password when doing commands.

***
## __Optimizing Remote Running__

- We can use quotation marks for commands directely `ssh` command, so that we can run them directely: 

such as `ssh cs15lwi22***@ieng6.ucsd.edu "ls"`
- We can also use semicolons to run multiple commands: 

`ssh cs15lwi22***@ieng6.ucsd.edu javac WhereAmI.java; java WhereAmI`

- However, by doing that, `java` command will run on client; `javac` command will run on server.
- To let both run on server, we can run the command:

`ssh cs15lwi22***@ieng6.ucsd.edu "javac WhereAmI.java; java WhereAmI"`

![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab1-Optimizing%20Remote%20Running.jpeg?raw=true)