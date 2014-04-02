---
layout: post
title:  "My own linux memo"
description: "some linux commands I found useful"
date:   2014-03-28 20:33:00
categories: tech
---

some linux commands I found useful

[A useful website that explains flag one by one](http://explainshell.com/)

* None can remember all, so we ["cheat"](https://github.com/chrisallenlane/cheat)!

* find:  
{% highlight bash %}
find PATH OPTION [-exec COMMAND { } \;]  
find / -type f -mtime -7 | xargs tar -rf weekly_incremental.tar   
find . \(-name a.out -o -name ‘*.o’\)> -atime +7 -exec cat {} \;   
find PATH1 PATH2 OPTION |	egrep "pattern"  
find –name "filename-with-wildcard"  
find !–name "filename-with-wildcard-that-want-exclude"  
find / -mmin -10   
-d[peth]   
-type x [df]
{% endhighlight %}

* egrep:  
{% highlight bash %}
egrep -r "text1|text2” directory-path 
egrep "text string to search” directory-path     
egrep -r "redeem reward" /home/tom/  
-E, --extended-regexp  egrep  
-F, --fixed-strings  fgrep 
{% endhighlight %}

* ls -lha
   ls -R 

* unzip *.zip

* git clone  user_name@cs1520.cs.pitt.edu:public/csweb  
   git clone --bare URL 

*  text replacing
{% highlight bash %}
#replace the 'f**k' of all text files in the directory with "lovely"     
find . -type f  |egrep "\.txt$" |xargs sed -i -e 's/fuck/lovely/g'  
#replacing with Chinese word is also feasible  
find . -type f  |egrep "\.txt$" |xargs sed -i -e 's/fuck/亲爱的/g'  
#having zero-extension ‘’ after -i will have no backup, as sed -i '' -e 'patten'  
{% endhighlight %}

* mkdir -p a/long/directory/path
  Make directory including intermediate directories

* cd -
  change to the previous working directory

*  $_ or !$: the last argument of the previous command.
   Ctrl+U to clear up to the beginning.
   Ctrl+K to delete to the end of line
   Ctrl+Y yank


    

