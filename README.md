# apaheTutorial
sudo yum install httpd -y // -yは全部yesの意味.  
sudo systemctl start httpd // systemctlはLinuxのコマンド。httpd(Apache)を起動.  
sudo systemctl enable httpd.service // サーバー起動時に自動的にApacheが起動するように設定.  
sudo usermod -a -G apache ec2-user //.  
sudo chown -R ec2-user:apache /var/www //.  
sudo chmod 2775 /var/www && find /var/www -type d -exec sudo chmod 2775 {} \; //.  
find /var/www -type f -exec sudo chmod 0664 {} \; //.  

