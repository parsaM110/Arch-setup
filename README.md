```
sudo pacman -S archlinux-keyring
```
update :
```
sudo pacman -Syu 
```
```
 sudo poweroff
```
install XFCE
```
sudo pacman -S xorg
sudo pacman -S xfce4 xfce4-goodies
pacman -Q 
sudo pacman -S lightdm lightdm-gtk-greeter
sudo systemctl enable lightdm
sudo reboot
```
install some core utiltiy
```
sudo pacman -S git
sudo pacman -S firefox
sudo pacman -S neofetch
sudo pacman -S python
sudo pacman -S python-pip
```
~~sudo pacman -S python-virtualenv~~ (use pyenv-virtualenv instead)
```
sudo pacman -S pyenv
```
install nessary tools for building python image
```
sudo pacman -S gcc
sudo pacman -S make
sudo pacman -S tk
```
install pyenv-doctor to checkout possible issues:
```
git clone https://github.com/pyenv/pyenv-doctor.git $(pyenv root)/plugins/pyenv-doctor
pyenv doctor -c -v
```
install python version:
```
pyenv install 3.11.1
```
see python versions:
```
pyenv versions
```
install  pyenv-virtualenv
```
git clone https://github.com/pyenv/pyenv-virtualenv.git $(pyenv root)/plugins/pyenv-virtualenv
pyenv virtualenv 3.11.1 venv
```
add these lines to .bashrc :
```
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
```
now run :
```
pyenv activate venv
```
deactivate:
```
deactivate
```
Delete Virtual Environment
```
pyenv virtualenv-delete <venv-name> 
```
after pip installign necessary packages, run:
```
streamlite run <.py file>
```





