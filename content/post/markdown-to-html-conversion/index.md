---
title: Markdown to Html Conversion
subtitle:  A simple code to convert markdown to html

summary: A simple code to convert markdown to html

draft: false
date: 2023-12-30T14:22:57+05:30
lastmod: 

categories:
    - Pandoc
tags:
    - Linux
    - Pandoc
    - Markdown
projects: []
featured: false
# authors:
#   - Ukant Jadia


image:
  caption: ''
  focal_point: ''
  placement: 2
  preview_only: false
---



# Conversion of Markdown(.md) to html markup language 

* get the `pandoc`  
* Use the following command 

```r
    pandoc smaple_readme.md -t html -o sample_readme.html
```

* In shell it would be written like 

```shell
cat=$(pandoc $1.md -t html -o $1.html )
```

* It will be run the loop with wildcard like 

```shell
  for i in ~/locat/.md/file/* ; do $(var) ; done 
```

# Modification 

* check extension of each file with if condition and print the non md file
  like 

```8ishell
if [ $1 -ne *.md ]
then 
    echo "UNEXPECTED Document format $1 "
    continue 
else:
    `further code`
fi

```
