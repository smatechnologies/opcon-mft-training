---
sidebar_label: 'File Renaming'
---

# File Renaming

Renaming of files performs a filename search and replace on the files within the file set using regular expressions. 

![RenameFiles](../../static/img/destination.png)

* **Search Pattern** 
  * Contains the regular expression to match
* **Replace Pattern** 
  * Contains the regular expression to replace.


:::tip Example 1

We use a Regular Expression to change the extension of the files in the file set from .txt to .dat.

* **Search Pattern**: ```^(.*)\.[^.]+$```
* **Replace Pattern**: ```"${1}.dat"```
:::

:::tip Example 2

We use a Regular Expression to add a date directory (date format can be defined using tokens) the files in the file set use the following definitions:

* **Search Pattern**: ```\\output\\(.*)$```
* **Replace Pattern**: ```"\\output\\[[$SCHEDULE DATE-YYYYMMDD]]\\${1}"```
:::