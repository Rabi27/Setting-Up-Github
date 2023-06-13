## Generate an SSH key pair
If you don't already have an SSH key, you can generate one by following the instructions over [here.](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

## Adding the SSH key to Github account
Add the SSH public key to your account on GitHub. Link over [here.](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

## Change the Origin
Follow the following steps:

- Verify your current remote origin by running the following command:
```bash
git remote -v
```
This will display the current remote URLs for fetching and pushing

- Remove the existing remote origin by running the following command:
```bash
git remote remove origin
```

- Add the new remote origin using the clone URL you provided:
```bash
git remote add origin <repository-url>
```
It is the URL you would use to clone the repository or interact with it remotely.

## Managing Different Email Accounts for Repository Access
To handle the situation where you have access to the repository using a different email account:

- On your local machine, open the terminal and navigate to the repository directory.
- Run the following command to set your email address for the specific repository:
```bash
git config user.email "your-email@example.com"
```
Replace `your-email@example.com` with the email address associated with the account that has access to the repository. This will ensure that your commits are attributed to the correct email address when interacting with this specific repository.
