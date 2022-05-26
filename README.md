# Windows 10 - VSCode Cheatsheet

# Useful shortcuts
<pre>
cntl + `     Opens/closes terminal window
F1           Opens command palette (easiest)
Ctrl+Shift+P Opens command palette (not sure why, but everyone uses this instead of F1)

</pre>

# Enabling tab completion
<pre>
$ touch ~/.bashrc
$ terraform -install -autocomplete

Once the autocomplete support is installed, you will need to restart your shell.
</pre>
# Sample .ssh/config file
<pre>
Host MyCustodianC7N-ORG
  HostName a.b.c.d
  User ubuntu
  IdentityFile "C:\Users\David Lin\.ssh\your_private_ssh_key.pem"
</pre>

