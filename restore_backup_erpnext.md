# Restore erpnext Backup


copy file to VM 
1. extract zip file
2. delete old database `drop database db-name`
3. your working directory should be main application directory
4. restore database 
    
       `bench --site your-site-name --force restore your-database-file-name.sql`
5. replace with your old encryption key 

## Extract gz file 

     gzip -d filename.gz

## extract tar file 
   
      tar xvf file.tar




