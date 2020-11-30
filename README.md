# Pre-requisites
Install the following programs:
- Vagrant
- VitualBox
- Ruby
- Bundler - manager for ruby app gems(formatted ruby programs and libs) manager

## Step by step set-up guide

1. Clone repo
2. In your terminal access the folder with cloned repo
```
cd <foldername>
```
3. Verify path correctness to ensure folder contains Vagrantfile
```
ls -a
```
4. Create and configure guest machine according to the Vagrantfile
```
vagrant up
```

- The app is now running
```
ip: 192.168.10.100
```
- The databse is now running
```
p: 192.168.10.200
```
- Enter the virtual machine
```
vagrant ssh app
```
- Inside the irtual machine run
```
cd /home/ubuntu/app
sudo npm install
sudo npm start
```

## View website
- Paste the following in your browser to view the pages
1. 192.168.10.100:3000
2. 192.168.10.100:3000/fibonacci/{index}
2. 192.168.10.100:3000/posts