# Cron-Job
How to schedule script using cron job.

## Check status of cron tab
    service cron status
    
## Start the cron service
    service cron start
    
## Restart the cron service
    service cron restart
  
## Stop the cron service
    service cron stop

## To view the list of existing cron jobs in your crontab
    crontab -l

## Access the cron table. Use the following command to open the cron table for editing
    crontab -e

- ``` * * * * *  command to execute
   ┬ ┬ ┬ ┬ ┬
   │ │ │ │ │
   │ │ │ │ │
   │ │ │ │ └───── day of week (0 - 7) (0 to 6 are Sunday to Saturday, or use names; 7 is Sunday, the same as 0)
   │ │ │ └────────── month (1 - 12)
   │ │ └─────────────── day of month (1 - 31)
   │ └──────────────────── hour (0 - 23)
   └───────────────────────── min (0 - 59) ```

- Command to write Hello in output.txt in a file every minute:

      ***** echo "Hello" >> /home/output.txt
