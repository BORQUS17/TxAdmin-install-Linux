[ PL ]
1. Do tej czyności potrzebujesz VPS lub Dedyka z systemem Linux.
2. Logujemy się do PUTTY za pomocą IP, root, Hasło root.
3. Jeżeli się zalogowałeś to wykonuj następujące komendy w PUTTY.

apt-get install git apache2 mysql-server phpmyadmin  ( Instalujemy wszystko zgodnie z Instrukcją )

apt-get update && apt-get upgrade  

cd ~

cd /home/

(Jeżeli mamy link do najnowszych artefaktów to pobieramy za pomocą putty tą komendą)  wget https://runtime.fivem.net/artifacts/fivem/build_proot_linux/master/5848-4f71128ee48b07026d6d7229a60ebc5f40f2b9db/fx.tar.xz

mkdir hees

tar -xvf fx.tar.xz -C /home/hees/

mkdir server

git clone https://github.com/citizenfx/cfx-server-data.git server

apt-get install screen

4. Logujesz się teraz do plików SFTP z pomocą ( winsoc, filezilla )
5. Wchodzisz w pliki /home/server/  i tam wgrywasz swoją paczke

########################## WŁAŚNIE POPRAWNIE SKONFIGUROWAŁEŚ SWÓJ SERWER ############################

1. Logujemy się do PUTTY

2. ( wpisujesz komende )  screen -dmS serwerfivem bash /home/server/run.sh

3.  ( A na sam koniec ) screen -r serwerfivem

Nie Klikaj Ctrl + C ponieważ wyłączysz cały serwer poprostu zamknij okno PUTTY
