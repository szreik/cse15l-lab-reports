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

`ssh cs15lsp22zz@ieng6.ucsd.edu`

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
