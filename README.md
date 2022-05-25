# Config Git Bash for Multiple GitHub Accounts

## Note: 
  - Should config in local for each repo
  - Can solve the error: "Permission to _github-repo_ denied to _username_"

## Steps 
_Note: All these commands work for working local repo_ 
1. Check the git config in local: `git config --local --list`
2. Config these things:
    - user name: `git config user.name "your-name"`
    - user email: `git config user.email "your-email"`
    - Windows Credential Manager(WCM): `git config credential.helper wincred`
    - Enable WCM for multiple credential: `git config credential.useHttpPath true`
3. Restart for applying
4. Check step 1 again to ensure proper info
5. Pull/push code using git
6. It's gonna to ask for logging in the Github you want to use
  - log in as normally
  - you can also use personal access token here:
    - go to: https://github.com/settings/tokens
    - generate one and paste it into the sign in box
7. If you want to check Windo(WCM): 
    - In Windows Search bar: enter `credential manager`
    - choose Windows Credentials tab
    - check if your github accounts exist here
  
  Yayyy now you can use differrent github account for each repo on your local machine =)))
