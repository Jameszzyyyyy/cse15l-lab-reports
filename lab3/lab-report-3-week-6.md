__CSE 15L Lab Report-2-week4__
=========
## Ziyou Zhao ziz021@ucsd.edu

***
## _**`.ssh/config` file**_
![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab3/lab3-config.png?raw=true)

- In the terminal, use command `cd ~/.ssh` to change to SSH directory.
- Type `nano config` to create a config file using nano.
- In the file, add 
    ```
    Host ieng6
        HostName ieng6.ucsd.edu
        User cs15lwi22zzz (use your username)
        IdentityFile ~/.ssh/id_rsa_ucsd
    ```
- Save the change.

***
## _**`ssh` command logging to acount**_
![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab3/lab3-ssh.png?raw=true)

- Use `ssh` command with the alias you chose(I chose "UCSD").
- Enter the password, and then you should be able to log into the account.

***
## _**`scp` command copying a file to acount**_
![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab3/lab3-WhereAmI.png?raw=true)
![Image](https://github.com/Jameszzyyyyy/cse15l-lab-reports/blob/main/lab3/lab3-scp.png?raw=true)

- Use `scp` command in local directory with the file name and the alias you chose(I chose "UCSD").
- Enter the password so that you can copy the file to the account.

