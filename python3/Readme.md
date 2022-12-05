![Screenshot_195](https://user-images.githubusercontent.com/81378817/205686379-8576a2c5-8249-496e-8469-b8d1b2a050f0.jpg)

this issue will shown when you remove python3 folder without purge/remove 


```bash
sudo apt purge python3
```
```bash
sudo apt-get purge python3
```

it take minutes
after few minuste you will see like

![Screenshot_196](https://user-images.githubusercontent.com/81378817/205687202-9e14f78a-a0b3-4ef9-a513-d4fbf9681912.jpg)

now install python3 again
```bash
sudo apt-get install python3
```
replace 3.8 with python version
```bash
sudo apt-get -y purge python3.8
sudo apt-get -y autoremove
```
the reinstall python3

```bash
wget https://www.python.org/ftp/python/3.8.0/Python-3.8.0.tgz
tar xzf Python-3.8.0
cd Python-3.8.0
sudo ./configure --enable-optimizations
sudo make altinstall
```
and install 
```bash
sudo apt update
sudo apt install build-essential zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev libssl-dev libreadline-dev libffi-dev wget
sudo make altinstall
```
and run again, please choose N for all questions
```bash
sudo apt -y install checkinstall
sudo checkinstall
```
then 
```bash
dpkg -r python
```
it will take some times 

thank you hopefull can help 
feel free to give me other suggestion to fix some problem

