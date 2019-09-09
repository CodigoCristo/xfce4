# xfce4-arch
Escritorio Xfce4

El microcódigo se puede actualizar a través de BIOS, 
El kernel de Linux también puede aplicar estas actualizaciones
durante el arranque. 
Estas actualizaciones proporcionan correcciones de errores 
que pueden ser críticas para la estabilidad de su sistema.

pacman -S amd-ucode

pacman -S intel-ucode

pacman -S lsb-release os-prober

Programa de consulta de versión LSB

pacman -S xdg-user-dirs
xdg-user-dirs-update

pacman -S xorg xorg-apps xorg-xinit xorg-twm xterm xorg-xclock
startx

Instalacion del servidor X

Driver Video
        lspci |grep VGA
        neofetch
        
pacman -S virtualbox-guest-utils 
systemctl enable vboxservice
        

pacman -S xfce4 xfce4-goodies network-manager-applet

pacman -S pulseaudio pavucontrol

pacman -S lightdm lightdm-gtk-greeter lightdm-gtk-greeter-settings 
systemctl enable lightdm

pacman -S chromium vlc gnu-free-fonts ttf-hack ttf-inconsolata 

git clone https://aur.archlinux.org/yay.git
cd yay/
makepkg -si






localectl --help
localectl set-x11-keymap latam
