# VSCode Cheatsheet

## Useful shortcuts
<pre>
Ctrl + `           Opens/closes terminal window
Ctrl + B           Toggles File Explorer pallete (Requires addition setting to work in terminal; see below for details)
Ctrl + P           Command pallete (file search)
F1                 Opens command palette (easiest)
Ctrl + Shift + P   Opens command palette (not sure why, but everyone uses this instead of F1)
Ctrl + Shift + V   View Markdown as webpage
Alt + up/down      Moves entire line up/down
Ctrl + Enter       Moves cursor to next line
Ctrl + '           Moves cursor outside last quotation mark
</pre>

## Useful Toggle pallette commands
```
toggle sidebar position
toggle vim mode
```


## How to update settings.json
Ctrl + P --> type "open user settings (json)"


## Enabling ability to toggle primary sidebar using Cntl + B when in terminal window
F1 --> Preferences: Open User Settings (JSON)
![image](https://github.com/davidclin/vscode-cheatsheet/assets/6853545/feaf1423-cd0b-4fb1-b579-72a9fb5ffd40)

## Enabling Bracket Pairs
File --> Preferences --> Settings --> Search for "pair bracket"
![image](https://github.com/davidclin/vscode-cheatsheet/assets/6853545/d1fe28cb-8478-49f5-8f5a-a32fb80c7a46)


## Disabling Ctrl+v in vscode terminal so VIM will work
Ctrl+V is binded to workbench.action.terminal.paste and this is one of default actions whose keybinding will be intercepted and handled by VS Code. Use next setting to exclute it from the list (will effectively disabled paste with Ctrl+V to the terminal)

"terminal.integrated.commandsToSkipShell": [
    "-workbench.action.terminal.paste"
]


## Enabling Terraform tab completion
<pre>
$ touch ~/.bashrc
$ terraform -install-autocomplete

Once the autocomplete support is installed, you will need to restart your shell.
</pre>

## Sample .ssh/config file
<pre>
Host MyCustodianC7N-ORG
  HostName a.b.c.d
  User ubuntu
  IdentityFile "C:\Users\David Lin\.ssh\your_private_ssh_key.pem"
</pre>
