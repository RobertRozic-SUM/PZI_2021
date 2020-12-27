# Programiranje za internet

## Deploy projekta na studentski server

### 1. SSH spajanje na studentski poslužitelj

Host: studenti.sum.ba
Username: fpmozXXYYYY
Password: csgiditalYYYY
Port: 22

*(XX broj grupe, YYYY godina)

    ssh fpmoz002021@studenti.sum.ba

- Ukoliko koristite windows, koristiti ssh klijent npr. Putty

### 2. Unutar početnog foldera klonirati projekt

    git clone https://github.com/RobertRozic-SUM/PZI_2021.git

### 3. Kreirati soft link sa public foldera projecta na public folder na poslužitelju

    ln -s /home/fpmozXXYYYY/ime-projekta/public  /home/fpmozXXYYYY/public
        
*Ukoliko naredba javi da file vec postoji, odradite:

    rm -rf ~/public
        
Pa zatim prethodnu naredbu

### 4. Aplikacija bi trebala biti dostupna na linku

https://studenti.sum.ba/projekti/fpmoz/YYYY/gX

npr. https://studenti.sum.ba/projekti/fpmoz/2021/g0/
