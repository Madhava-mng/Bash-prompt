# Bash-prompt
bash prompts orignal and duplicates 

### Glowin
##
    NOTE:
      1) open  ~/.bashrc
      2) past the particular code at the end of the "~/.bashrc" file
      3) specify your user name(directory) at "<USER>" this area
 

```bash
# Glowin-basic from Bash-prompt 
export HOME=/home/<USER>/../<USER>
PS1='\[\033[32;1m\]($(ym=$?;if [ $ym -ne 0 ];then printf "\[\033[31;1m\]$ym ";fi)\[\033[1;32;1m\]\W)\[\033[35m\] 》\[\033[00m\]'
```

```bash
export HOME=/home/<USER>/../<USER>
PS1='$(ym=$?;if [ $ym -ne 0 ];then printf "\[\033[31;1m\]($ym)";fi)\[\033[1;34;1m\](\W)\[\033[35m\] 》\[\033[00m\]'
```

```bash
export HOME=/home/<USER>/../<USER>
PS1='$(ym=$?;if [ $ym -ne 0 ];then printf "\[\033[31;1m\]$ym << ";fi)\[\033[1;32;1m\](\W)\[\033[35m\] 》\[\033[00m\]'
```

```bash
export HOME=/home/<USER>/../<USER>
PS1='\[\033[32;1m\](\t)-$(ym=$?;if [ $ym -ne 0 ];then printf "\[\033[31;1m\]($ym)-";fi)\[\033[1;32;1m\](\W)\[\033[35m\] 》\[\033[00m\]'
```

```bash
export HOME=/home/<USER>/../<USER>
PS1='$(if [ $? -ne 0 ];then printf "\[\033[31;1m\](\W)";else printf "\[\033[1;32;1m\](\W)";fi)\[\033[35m\] 》\[\033[00m\]'
```

### Airline 
```bash
export HOME=/home/<USER>/../<USER>
END=""
PS1='$(ym=$?;if [ $ym -ne 0 ];then printf "\[\033[41m\]\[\033[37;1m\]$ym\[\033[0m\]\[\033[31;1m\]\[\033[44m\]$END";fi)\[\033[44m\]\[\033[37;1m\]\W\[\033[0m\]\[\033[34m\]$END\[\033[00m\] '
```

