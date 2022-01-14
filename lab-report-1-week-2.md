# Lab Report 1 Week 2

## Including Screenshots

This is a screenshot of the secondary file we made during discussion on 1/13/22

![Image](test_screenshot.jpg)

## Tutorial for how to log into a course-specific account on ieng6

1. *Installing VScode*

    Go to the Visual Studio Code website to download VScode [https://code.visualstudio.com/](https://code.visualstudio.com/)

---

2. *Remotely connecting*

    First, install OpenSSH, which allows you to connect to the UCSD servers: [OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)

    I'm on Windows 10 so I just followed the instructions on the link above.

    ![Image](images/install_openssh_instructions.png)
    ![Image](images/installed_openssh_settings.png)

    Next, look up your course specific account for CSE15L at this link: 

    [https://sdacs.ucsd.edu/~icc/index.php](https://sdacs.ucsd.edu/~icc/index.php)

    I had a lot of problems finding my login info and then trying to connect to the server from here though -- if this happens, you may need to reset your password (I did this three times before getting positive results).

    ![Image](images/account_lookup_results.png)

    Your account should start with `cs15lwi22`. Now go open up a terminal in VScode, and connect to the remote server by typing `ssh cs15lwi22abc@ieng6.ucsd.edu` into the terminal, where `abc` is your specific account. 

    Hopefully, you should get something like this after typing in your password:

    ![Image](images/connected_to_remote_server.png) 

    If you get a message asking about authenticity, just say yes.

    **NOTE:** I had an error that was apparently pretty common, where when typing in my password it wouldn't go through 3 times. Then it would ask for the password to the server, and after a few more tries it would not connect. I'm not sure what the solution is but it was fixed after a day of changing my password.

---

3. *Trying some commands*

    

4. *Moving files with* `scp`
5. *Setting an SSH key*
6. *Optimizing remote running*

