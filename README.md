# docker-php7_apache-mariadb  

**โครงสร้าง**  
```
.
+-- compose
    -- docker-compose.yml
+-- site
    -- index.php
```


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