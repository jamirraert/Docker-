## Christian Fernan ##

INSTALL DOCKER SERVER

### UBUNTU SERVER ###
1. Update system to latest package information:
```
sudo apt update
```

2. Install Dependencies:
```
sudo apt install -y apt-transport-https ca-certificates curl software-properties-common
```

3. Add the Docker GPG key:
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```

4. Set Up the Stable Docker Repository
```
echo "deb [signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

5. Update the Package Database Again:
```
sudo apt update
```

6. Install Docker:
```
sudo apt install -y docker-ce docker-ce-cli containerd.io
```

7. Check if success docker installation
```
sudo docker run hello-world
```

