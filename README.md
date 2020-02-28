Vaja 8 CubeMX


2.

c) V pinout zavihku omogočite I2C komunikacijo. Kateri pini se aktivirajo?
   - Aktivirata se pina "PB6" ter "PB7".
   Koliko različnih komunikacij vaša razvojna plošča omogoča?
   - Omogoča 3 različne komunikacije.

e) ADS1115 modul povežite z ustreznimi pini na STM32F0.
   - PB6-SCL | PB7-SDA | 5V-VDD | NC-ALRT | GND-ADDR.

f) V zavihku Configuration za I2C spremenite hitrost na 400 kHz. Kaj ste izbrali?
   - Izbral sem "Fast mode".


3.

c) Pretvorite binarni naslov 1001000 v šestnajstiškega.
   - To je 48 hex.

f) ADS pretvorniku moramo programsko nastaviti vhodno ojačanje (programmable gain amplifier configuration).
   Ker so naše vrednosti na potenciometru do 5 V, moramo ustrezno postaviti 16-bitni register - bite od 11:9 postavimo na 000.
   Koliko je max. napetost?
   - Maksimalna napetost je 6,144 V.


Komentar:
 - Že pred začetkom opravljanja vaje sem preveril GitHub od sošolcev in sem opazil, da vaja ne deluje z STM Discovery ploščo.
   Zato sem takoj uporabil ploščo Nucleo-L476RG in delovalo je kot mora.
