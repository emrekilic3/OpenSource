# Acik_kaynak_BC_HW_2
1) Download and install apache2

```bash
sudo apt update
sudo apt install apache2
```
2) Change directory to /var/www/html

```bash
cd /var/www/html
```

3) Create new HTML file and configure it with Nano text editor

```bash
sudo touch havelsanHW2.html
sudo nano havelsanHW2.html
```
4) Check the current status of your apache server

```bash
sudo systemctl status apache2	
```
5) See latest 20 logs of access.log and error.log

```bash
tail -f -n 20 /var/log/apache2/access.log /var/log/apache2/error.log
```
6) Configure apache2 using Nano text editor

```bash
sudo nano /etc/logrotate.d/apache2
```
```bash
/var/log/apache2/*.log {
        hourly
        missingok
        rotate 20
        compress
        create
        postrotate
                service apache2 restart
        endscript

}
```
7) Compress logs using logrotate command

```bash
sudo logrotate -f /etc/logrotate.d/apache2
```
