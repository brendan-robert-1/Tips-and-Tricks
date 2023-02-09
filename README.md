# Tips-and-Tricks
bunch of developer tips 


## Git

*Multiple git accounts same machine*

 `git config --local credential.helper ""`
 
  `git push origin master`
  
  This is a last ditch effort to push changes when you absolutely need to and cant figure out ssh stuff. 
  
  The correct way to do it is detailed: https://gist.github.com/rahularity/86da20fe3858e6b311de068201d279e3
  
  The issues with this way is that if your `~/.ssh/config` file has a `Host` that is wildcarded (not sure why but mine is on some machines) I dont think git will resolve the correch ssh key and just pick that one every time.
