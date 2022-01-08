# Ubuntu-Could-not-get-lock-var-lib-dpkg-lock-frontend
Ubuntu Could not get lock /var/lib/dpkg/lock-frontend

```
sudo killall apt apt-get
```

If none of the above works, remove the lock files. Run in terminal:
```
sudo rm /var/lib/apt/lists/lock
sudo rm /var/cache/apt/archives/lock
sudo rm /var/lib/dpkg/lock*
```

then reconfigure the packages. Run in terminal:
```
sudo dpkg --configure -a
sudo apt update
```
