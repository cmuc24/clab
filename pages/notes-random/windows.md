# Windows

Wie in Windows fast immer, schneller gehts mit fetzigen GUIs
https://www.heise.de/download/product/link-shell-extension-39057


```shell script copy
Symlinks in Windows 
# target is a directory, create junction
"mklink /j `"$source`" `"$target`""

# target is a file, create hard link
"mklink /h `"$source`" `"$target`"" 
```


```shell script copy
# target is a directory, create junction
New-Item -Path $source -ItemType Junction -Value $target

# target is a file, create hard link
New-Item -Path $source -ItemType HardLink -Value $target | Out-Null
```
