# How to log uptime with crontab and uptime command  

Today, I learned how to append a log of uptime to a texfile and run it periodically

 - To write uptime of a machine use command 
```bash
update
```
 - To append the output of a command use >> 
 
      _uptime >> ~/uptime_log.txt_

 - To schedule this command to run every 10 minutes use crontab -e and write the following to your cronfile 
     
      */10 * * * * uptime >> ~/uptime_log.txt
or 
     
     0,10,20,30,40,50 * * * * uptime >> ~/uptime_log.txt

