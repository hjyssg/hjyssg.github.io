---
layout: post
title:  "My own linux memo"
description: "some linux commands I found useful"
date:   2014-03-28 20:33:00
categories: tech
---

some linux commands I found useful

[A useful website that explains flag one by one](http://explainshell.com/)

1. None can remember all, so we ["cheat"](https://github.com/chrisallenlane/cheat)!

1. find:  
	
		find PATH OPTION [-exec COMMAND { } \;]  
		find / -type f -mtime -7 | xargs tar -rf weekly_incremental.tar  
		find . \(-name a.out -o -name ‘*.o’\)> -atime +7 -exec cat {} \;   
		find PATH OPTION |	grep "pattern"  
		find –name "filename-with-wildcard"  
    	find !–name "filename-with-wildcard-that-want-exclude"  
    	find / -mmin -10   
    	-d[peth]   
    	-type x [df]
	


1. egrep:  

		egrep -r "text1|text2” directory-path 
		egrep "text string to search” directory-path     
		egrep -r "redeem reward" /home/tom/  
		-E, --extended-regexp  egrep  
		-F, --fixed-strings  fgrep  

1. ls -lha
   ls -R 

1. unzip *.zip

1. git clone  user_name@cs1520.cs.pitt.edu:public/csweb  
   git clone --bare URL 
