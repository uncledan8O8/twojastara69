<br />
#==========================================#<br />
#============ PRZYGOTOWANIA ==============#<br />
#==========================================#<br />
<br />
sudo apt update && sudo apt upgrade -y<br />
sudo apt install unzip git<br />
git clone https://github.com/uncledan8O8/twojastara69.git<br />
unzip ~/twojastara69/vpn.zip<br />
#--------- HASŁO JAK DO GHOSTA ------------#<br />
#==========================================#<br />
<br />
<br />
<br />
#/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\#<br />
<br />
<br />
<br />
#==========================================#<br />
#======= USTAWIANIE WIĘC SIĘ SKUP ========#<br />
#==========================================#<br />
<br />
sudo cp ~/twojastara69/vpn/poland/* /etc/openvpn<br />
sudo cp ~/twojastara69/vpn/ustawienia/openvpn /etc/default/openvpn<br />
sudo chmod 400 /etc/openvpn/poland.txt<br />
sudo mv /etc/openvpn/poland.ovpn /etc/openvpn/poland.conf<br />
sudo rm /etc/systemd/system/multi-user.target.wants/openvpn.service<br />
sudo cp ~/twojastara69/vpn/ustawienia/poland@service /usr/lib/systemd/system/<br />
sudo systemctl enable openvpn@poland.service<br />
sudo systemctl daemon-reload<br />
sudo systemctl start openvpn@poland.service<br />
sudo service openvpn@poland start<br />
sudo cp ~/twojastara69/vpn/ustawienia/poland /etc/init.d/<br />
reboot
<br />
<br />
#==========================================#<br />
<br />
<br />
<br />
#/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\#
<br />
<br />
<br />
#====== KOMENDA DO W(Y)ŁĄCZENIA VPN =======#<br />
     sudo service openvpn@poland stop<br />
#==========================================#<br />
<br />
<br />
#======== KOMENDA DO WŁĄCZENIA VPN ========#<br />
     sudo service openvpn@poland start<br />
#==========================================#<br />
<br />
<br />
<br />
#==========================================#<br />
#===========>  UNCLE DAN(c)  <============#<br />
#==========================================#<br />
<br />
