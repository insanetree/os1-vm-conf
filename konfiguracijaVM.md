# Konfiguracija

## Uvod
Ovo je pokusaj rekonstrukcije svih stvari koje treba uciniti u svom Linux sistemu kako bi se mogao pisati projekat van virtuelne masine. U sustini samo sam kopao po log fajlovima i gledao sta je sve Sustran radio.
Verujem da ce najbolje ovo raditi na Mintu, Ubuntu i ostalim Debian distribucijama, ali **NE GARANTUJEM DA CE RADITI BILO STA I DA CE NA ODBRANI SVE BITI U REDU**

Sudeci po log fajlovima, profesor je radio sve 2021-10-24

## Instalirani paketi
Izvor za ovo je fajl /var/log/apt/history.log

Ako pozelite da instalirate sve pakete, ispod je lista svega sto sam nasao. Imajte na umu da ce na vasoj distribuciji neki paketi imati drugo ime i budite spremni na moguce komplikacije.

- git (ne znam zasto je ovo instalirao)
- build-essential
- qemu-system-misc
- gcc-riscv64-linux-gnu
- binutils-riscv64-linux-gnu
- gdb-multiarch
- g++-riscv64-linux-gnu

Komanda za instalaciju na Ubuntu sistemu je sledeca:
>`sudo apt install git build-essential qemu-system-misc gcc-riscv64-linux-gnu binutils-riscv64-linux-gnu gdb-multiarch g++-riscv64-linux-gnu`

## Zavrsna rec
Vrlo je verovatno da je nesto skidano sa githuba, ali stvarno sumnjam da je bilo sta od vaznosti za izradu projekta. Prosao sam kroz Makefile i u sustini je sve tu na mestu i mislim da je sve odozgo dovoljno za uspesno prevodjenje vaseg koda.

## TODO
- [ ] testirati da li je moguce kompajlovati kod na fizickoj masini posle instaliranih paketa
- [ ] videti da li je jos nesto radjeno
- [ ] eventualne izmene fajla