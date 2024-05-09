# orai-disk-space

STEP:1
disk-space-script.sh file:

Run the following command to make executable file:
sudo chmod +x disk-space-script.sh

STEP:2
Script to check the disk space every 6 hours:

sudo chmod +x check_disk_script.sh

STEP:3
Create a Crontab Scheduler:

Runt the following command on your server and follow theinstructions:

crontab -e

Add the following lines

##Check disk space every 6 hours

0 */6 * * * /$HOME/check_disk_script.sh
