# setup a nextcloud with docker-compose

# rsync -avz -e 'ssh' ./nextcloud bill@192.168.100.201:/home/bill/

sudo apt update && sudo apt install docker.io docker-compose
sudo usermod -aG docker $USER
sudo reboot
docker --version
cd nextcloud/
#docker-compose up
nohup docker-compose up &
