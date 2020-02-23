# AdrielFreud
![](https://img.shields.io/badge/Programming-a-EPROM-(bios)-blue)

 - Requisições Web e Extração de Dados

# Circuito Proto-Board
![photo](https://eletronicabr.com/uploads/monthly_2015_12/Serduino_fritzing.jpg.9a8f060d155836c757a81618afee4ae1.jpg)


# Instalação
 - sudo apt-get update
 - sudo apt-get install flashrom
 - sudo apt-get install binutils gcc-avr avr-libc
 - sudo echo "deb sana main non-free contrib" >> ./etc/apt/sources.list
 
 - git clone --recursive git://github.com/urjaman/frser-duino
 - cd frser-duino
 
# Para fazer backup da bios digite:
  - flashrom -p serprog:dev=/dev/ttyACM0:115200 -r nome_do_backup.bin ou .rom

# Para gravar a bios digite:
  - flashrom -p serprog:dev=/dev/ttyACM0:115200 -w nome_do_arquivo.bin ou .rom

# Para apagar a bios digite:
  - flashrom -p serprog:dev=/dev/ttyACM0:115200 -E
# Para outras opções digite:
  - flashrom --help
