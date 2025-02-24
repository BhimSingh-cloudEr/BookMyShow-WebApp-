# Node js Project having Portfolio-Website 

#### Repo URL Below
[ref] - https://github.com/jaiswaladi246/Portfolio-Website.git

#### Download and install nvm:
	curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash

#### in lieu of restarting the shell
	\. "$HOME/.nvm/nvm.sh"

#### Download and install Node.js:
	nvm install 22

#### Verify the Node.js version:
	node -v 
		--> Should print "v22.14.0".
	nvm current
		--> Should print "v22.14.0".

#### Verify npm version:
npm -v 
		--> Should print "10.9.2".
		
		
		cd Portfolio-Website
		npm start
		npm run build
		cd /var/www/html
			sudo cp -r /home/ubuntu/Portfolio-Website/build .
		cd /etc/nginx/sites-available
		ls
			default
		sudo rm -rf default
		vi default
		
		-->			server {
								listen 80;
								server_name 13.126.250.70;
								root /var/www/html;
								index index.html;
								location / {
								try_files $uri /index.html;
										}
								}

### ubuntu@ip-172-31-12-185:~$ history
**
    1  sudo apt-get update
    2  ls
    3  cd Portfolio-Website/
    4  npm install
    5  sudo apt install npm
    6  npm start
    7  ls
    8  sudo npm install
    9  npm audit fix --force
   10  npm start
   11  sudo su -
   12  sudo update
   13  sudo apt update
   14  cd Portfolio-Website/
   15  ls
   16  npm start
   17  ls
   18  cd ..
   19  sudo chown 777 Portfolio-Website/
   20  cd Portfolio-Website/
   21  npm start
   22  cd ..
   23  sudo chown -R $USER:$USER ~/Portfolio-Website
   24  cd Portfolio-Website/
   25  npm start
   26  sudo systemctl restart
   27  reboot
   28  history
**


