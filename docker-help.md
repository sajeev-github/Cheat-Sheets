
Remove docker old instances
```
sudo apt-get remove docker docker-engine docker.io containerd runc
```

Install docker
```
 curl -fsSL https://get.docker.com -o get-docker.sh
 sudo sh get-docker.sh
 ```

Run with non-root previlege
```
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker
```

Start / Stop service
```
sudo systemctl enable docker.service
sudo systemctl enable containerd.service
```



