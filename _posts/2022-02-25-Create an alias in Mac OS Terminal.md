---
title:  "Create an alias in Mac OS Terminal" 
categories: [accessibility]
description: How to Create an alias in Mac OS Terminal
tags: [macos, keyboard-shortcuts]
--- 

Aliases can be handy while using Terminal in Mac OS.  
Alias is a shortform that we can use to execute a bigger more complex query.  

Here is how you can create alias to use in Mac OS Terminal.  

``` bash
cd ~
vim .bash_profile
# add/update alias
```

Update the file.

``` bash
alias c="clear"
alias som="some"
#...
```

_Please note that once you make this change you have to restart the Terminal._

## List all aliases

```bash
alias
```

This command will list all aliases registered in the Terminal.