# docker-php7_apache-mariadb  

**โครงสร้าง**  
```
.
+-- compose
    -- docker-compose.yml
+-- site
    -- index.php
```

#!/bin/bash

#File: tree-md

tree=$(tree -tf --noreport -I '*~' --charset ascii $1 |
       sed -e 's/| \+/  /g' -e 's/[|`]-\+/ */g' -e 's:\(* \)\(\(.*/\)\([^/]\+\)\):\1[\4](\2):g')

printf "# Project tree\n\n${tree}"

**Run Docker**  
``` 
& cd compose  
& docker-compose up
``` 
**Check Docker**  
``` 
& docker ps -a
```
**Database**  
```
& cd compose  
& docker-compose exec db bash  
& mysql -u root -p
```
```
> use yamroll;
```