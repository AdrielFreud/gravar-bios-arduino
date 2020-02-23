# AdrielFreud
![](https://img.shields.io/badge/Programming--a--EPROM--(bios)-blue)

 - Grave Sua EPROM (Bios) com arduino.

# Circuito Proto-Board
![photo](https://eletronicabr.com/uploads/monthly_2015_12/Serduino_fritzing.jpg.9a8f060d155836c757a81618afee4ae1.jpg)


# Instalação
 - sudo apt-get update
 - sudo apt-get install flashrom
 - sudo apt-get install binutils gcc-avr avr-libc
 - sudo echo "deb sana main non-free contrib" >> ./etc/apt/sources.list
 
 - git clone --recursive git://github.com/urjaman/frser-duino
 - cd frser-duino
 - make u2 && make flash-u2

# Para fazer backup da bios digite:
  - flashrom -p serprog:dev=/dev/ttyACM0:115200 -r nome_do_backup.bin ou .rom
  ![photo](https://i.imgur.com/ObhPQJl.png)


# Para gravar a bios digite:
  - flashrom -p serprog:dev=/dev/ttyACM0:115200 -w nome_do_arquivo.bin ou .rom
  ![photo](https://i.imgur.com/khCnKu6.png)


# Para apagar a bios digite:
  - flashrom -p serprog:dev=/dev/ttyACM0:115200 -E


# Para outras opções digite:
  - flashrom --help
