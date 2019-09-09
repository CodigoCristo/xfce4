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

-----------------------------------------------------------------------------------------------------

Organizar particiones:

sudo pacman -S android-file-transfer msmtp libmtp libcddb gvfs gvfs gvfs-afc gvfs-smb gvfs-gphoto2 gvfs-mtp gvfs-goa gvfs-nfs gvfs-google

Leer cualquier formato de disco:

sudo pacman -S dosfstools jfsutils f2fs-tools btrfs-progs exfat-utils ntfs-3g reiserfsprogs udftools xfsprogs nilfs-utils polkit gpart mtools

Compresión y Descompresión:

sudo pacman -S xarchiver binutils gzip lha lrzip lzip lz4 p7zip tar xz bzip2 p7zip lbzip2 arj lzop cpio unrar unzip zstd zip lzip unarj zstd 


CODEC DE AUDIO: 

sudo pacman -S pulseaudio pulseaudio-alsa pavucontrol pamixer pulseeffects pulseaudio-equalizer  lib32-alsa-plugins lib32-libpulse pulseaudio-equalizer-ladspa libcanberra-pulse libcanberra-gstreamer


CODEC DE VIDEO: 

sudo pacman -S ffmpeg aom libde265 x265 x264 libmpeg2 xvidcore libtheora libvpx schroedinger sdl gstreamer gst-plugins-bad gst-plugins-base gst-plugins-base-libs gst-plugins-good gst-plugins-ugly xine-lib libdvdcss libdvdread dvd+rw-tools lame

ffmpeg -formats -E

Codec de imagen

sudo pacman -S jasper openjpeg

-----------------------------------------------------------------------------------------------------

Para utilizar bashrc:
Copiar el contenido como root con "su"
y editamos texto

gedit .bashrc

copiamos texto de bashrc 
.bashrc 

para bashrc_root reemplazamos todo el texto en
sudo nano /etc/bash.bashrc 
nano ~/.bashrc_root 


Para utilizar zshrc:
sudo pacman -S zsh zsh-syntax-highlighting
Copiar el contenido de zshrc como root a .zshcr
sudo chsh -s /bin/zsh nombre_usuario

-----------------------------------------------------------------------------------------------------



