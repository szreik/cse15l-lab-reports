# Lab Report 1
## Installing VScode
1. Go to the [Visual Studio Code website.](https://code.visualstudio.com/)
2. Click the "Download" button pictured below, and choose the appropriate download corresponding to your operating system.
![Image](vscode.png)
3. Follow the application's instructions for installation.

## Remotely Connecting
1. If you are on Windows, install the [OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse) program. If you are on Mac, ignore this step and proceed to Step 2.
2. Look up your course specific account by entering the information on [this website](https://sdacs.ucsd.edu/~icc/index.php).
3. Open VScode and open a terminal by clicking "Terminal" in top menu and then selecting new terminal.
4.  Enter the following command into the terminal, replacing `XX` with the appropriate letters from your course specific account.

    `ssh cs15lsp22zXX@ieng6.ucsd.edu`

5. If you get a message that reads:

    `The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't
be established.
RSA key fingerprint is
SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting
(yes/no/[fingerprint])?`

    Enter `yes` into the terminal.

6. Enter your password, and if you see the following screen you are connected!
![Image](remotecon.png)

## Trying Some Commands
 1. Try the `ls -lat` and `ls -a` commands on the remote server.
 ![Image](lslat.png)
 2. Try the `cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/`  and ` cat /home/linux/ieng6/cs15lsp22/public/hello.txt` commands on the remote server.
 ![Image](cpcat.png)
 3. Try the `ls -lat` and `ls -a` commands on client.
 ![Image](lslatclient.png)
 4. Try the `cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/`  and ` cat /home/linux/ieng6/cs15lsp22/public/hello.txt` on client.
 ![Image](catclient.png)

## Moving Files With `scp`
1. Put java file (in this case, WhereAmI.java) onto your computer.
2. Enter

     `scp WhereAmI.java cs15lsp22XX@ieng6.ucsd.edu:~/` 
     
     into the terminal on client, again replacing `XX` with the appropriate letters from your course specific account.
3. Use ssh to enter remote server.
4. Use command `ls` to check if file (WhereAmI.java) is in ssh.
![Image](scp.png)

## Setting An SSH Key
