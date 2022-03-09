---
title:  "Reduce the path length in Linux Terminal" 
categories: [tips]
description: How to Reduce the path length in Linux Terminal
tags: [linux, terminal]
--- 

Lately I have been struggling with the strange scenario... of having to deal with too long a path.  
The trouble is the folder I'm mostly deeling with is too deep in.  
The prompt in the terminal gets too long, it ends up getting too cluttered.  
It makes it very difficult to read. All you see is the path.  

So, how do you deal with this.  

Very simple. Update the Prompt Dir Trim value.    
Go to the terminal and type the following.  

``` bash
PROMPT_DIRTRIM=1
```

This will limit the prompt to display only the last folder name preceeded by `...`  
If you feel it gives too less info on the path, you can change the number of directories to display by adjusting the value of PROMPT_DIRTRIM.

If you set `PROMPT_DIRTRIM=2`, it will display two directories.  
If you want to reset it to the original, just do `PROMPT_DIRTRIM= `.  
This will reset the prompt and display the complete path.  


At anytime, if you need to check the value of prompt. Do the following.
``` bash
echo $PROMPT_DIRTRIM
```

