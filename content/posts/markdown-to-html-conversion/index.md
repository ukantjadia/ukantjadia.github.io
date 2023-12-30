---
title: Markdown to Html Conversion
seo_title: Markdown to Html Conversion
summary: A simple code to convert markdown to html
description: A simple code to convert markdown to html
slug: markdown-to-html-conversion
author: Ukant Jadia

draft: false
date: 2023-12-30T14:22:57+05:30
lastmod: 
expiryDate: 
publishDate: 2022-06-26T22:47:32+05:30

feature_image: 
feature_image_alt: 

categories:
    - Pandoc
tags:
    - Linux
    - Pandoc
    - Markdown
series:

toc: true
related: true
social_share: true
newsletter: false
disable_comments: false
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
