# MHS-3.5inch RPi Display Screen

# Installation on Raspbian

```bash
sudo rm -rf LCD-show
git clone https://github.com/goodtft/LCD-show.git
chmod -R 755 LCD-show
cd LCD-show/
sudo ./MHS35-show
```

# Installation on Kali

```bash
sudo rm -rf LCD-show

# Official Repo
wget http://www.lcdwiki.com/res/MHS3528/kali-linux/LCD-show.tar.gz
# Or
# Use this Repo to fix kernel panic problem
wget https://github.com/danielcshn/LCD-show-kali.git
```
```bash
tar -xvzf LCD-show.tar.gz
chmod -R 755 LCD-show
cd LCD-show/
sudo ./MHS35-show
```
