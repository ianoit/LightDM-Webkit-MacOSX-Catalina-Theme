LightDM Webkit MacOSX Catalina Theme
===========================

Saya membuat ini berdasarkan [https://github.com/Wattos/LightDM-Webkit-MacOSX-Theme](https://github.com/Wattos/LightDM-Webkit-MacOSX-Theme), tetapi karena saya masih kurang sreg akhirnya sedikit saya ubah

## Screenshoot
![Screenshoot]()

## Installasi

1. Install git (if not installed). ```sudo apt install git```
2. Installed webkit-greeter (if not installed). ```sudo apt install lightdm-webkit-greeter```
3. ```cd ~/Downloads```
4. ```git clone https://github.com/Wattos/LightDM-Webkit-MacOSX-Theme```
5. ```cd LightDM-Webkit-MacOSX-Theme/```
6. ```sudo mkdir -p /usr/share/lightdm-webkit/themes/mac```
7. If /etc/lightdm/lightdm.conf does not exist, ```sudo bash -c 'echo "[SeatDefaults]" >> /etc/lightdm/lightdm.conf'```
8. ```sudo bash -c 'echo "greeter-session=lightdm-webkit-greeter" >> /etc/lightdm/lightdm.conf'```
9. ```sudo cp -rv * /usr/share/lightdm-webkit/themes/mac```
10. ```sudo sed -i 's/webkit-theme=default/webkit-theme=mac/' /etc/lightdm/lightdm-webkit-greeter.conf```
11. ```sudo reboot```

## Mengubah Gambar Background
1. Siapkan gambar yang ingin digunakan
2. Copy gambar ke folder assets/img
3. Buka file style.css di folder /assets/img
4. Edit pada bagian ```background-image: url("../img/bg.jpg");``` ubah bg.jpg dengan nama gambar kalian

Catatan:
Wallpaper : 
[https://wallpapershome.com/download-wallpapers/macos-catalina-day-mountains-wwdc-2019-5k-21590.html](https://wallpapershome.com/download-wallpapers/macos-catalina-day-mountains-wwdc-2019-5k-21590.html)