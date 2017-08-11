
[sed](http://sed.sourceforge.net/)


#### 把所有的行都归为一行:(即替换所有结尾的换行符\n)

> sed ':a;N;$!ba;s/\n/ /g' file.txt 

> sed '1~3d' file      		# delete every 3d line, starting with line 1, deletes lines 1, 4, 7, 10, 13, 16, ...
  sed '0~3d' file      		# deletes lines 3, 6, 9, 12, 15, 18, ...
  sed -n '2~5p' file   		# print every 5th line, starting with line 2, prints lines 2, 7, 12, 17, 22, 27, ...


