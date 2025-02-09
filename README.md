
#==========================================#<br />
#============ PRZYGOTOWANIA ==============#<br />
#==========================================#<br />

sudo apt update && sudo apt upgrade -y

sudo apt install unzip git

git clone https://github.com/uncledan8O8/twojastara69.git

unzip ~/twojastara69/vpn.zip
                   /\
                  /||\
                   ||
             ---------------
#--------- HASŁO JAK DO GHOSTA ------------#
#==========================================#



#/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\#



#===========================================#<br />
#======= USTAWIANIE WIĘC SIĘ SKUP =========#<br />
#===========================================#<br />

sudo cp ~/twojastara69/vpn/poland/* /etc/openvpn

sudo cp ~/twojastara69/vpn/ustawienia/openvpn /etc/default/openvpn

sudo chmod 400 /etc/openvpn/poland.txt

sudo mv /etc/openvpn/poland.ovpn /etc/openvpn/poland.conf

sudo rm /etc/systemd/system/multi-user.target.wants/openvpn.service

sudo cp ~/twojastara69/vpn/ustawienia/poland@service /usr/lib/systemd/system/

sudo systemctl enable openvpn@poland.service

sudo systemctl daemon-reload

sudo systemctl start openvpn@poland.service

sudo service openvpn@poland start

sudo cp ~/twojastara69/vpn/ustawienia/poland /etc/init.d/

reboot

#==========================================#<br />



#/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\#



#====== KOMENDA DO W(Y)ŁĄCZENIA VPN =======#<br />
     sudo service openvpn@poland stop
#==========================================#<br />


#======== KOMENDA DO WŁĄCZENIA VPN ========#<br />
     sudo service openvpn@poland start
#==========================================#<br />



#==========================================#<br />
#===========>  UNCLE DAN(c)  <============#<br />
#==========================================#<br />
