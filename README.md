# NOTES 
For configuring github access
////////////////////
cd ~/.ssh && ssh-keygen

Next you need to copy this to your clipboard.
On OS X run: cat id_rsa.pub | pbcopy
On Linux run: cat id_rsa.pub | xclip
On Windows (via Cygwin/Git Bash) run: cat id_rsa.pub | clip
On Windows (Powershell) run: Get-Content id_rsa.pub | Set-Clipboard (Thx to @orion elenzil)
Add your key to your account via the website.
Finally setup your .gitconfig.
git config --global user.name "bob"
git config --global user.email bob@... (don't forget to restart your command line to make sure the config is reloaded)
That's it you should be good to clone and checkout.

---
 ssh -T git@github.com
