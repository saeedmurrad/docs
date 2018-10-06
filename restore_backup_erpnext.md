# Restore erpnext Backup


Copy file to VM 
1. Extract zip file
2. Delete old database `drop database db-name`
3. Your working directory should be main application directory
4. Restore database 
    
       bench --site your-site-name --force restore your-database-file-name.sql
5. Replace with your old encryption key in site_config.json
6. Run migration command

        bench migrate
7. Delete All Email Accounts and make new Email Accounts
8. Enable Schedular for automation of email sending

        bench --site SITENAME enable-scheduler
## Extract gz file 

     gzip -d filename.gz

## extract tar file 
   
      tar xvf file.tar




