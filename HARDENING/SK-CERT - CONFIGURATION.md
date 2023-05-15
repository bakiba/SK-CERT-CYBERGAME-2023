# SK-CERT - CONFIGURATION
> Ste adminom web servera a prišlo Vám niekoľko požiadavok ohľadom zmien konfigurácií. Prikladáme celé /etc/ https://drive.google.com/file/d/1DtMrIe4i9Bn1UITyYEUZc_Je8QSDylb8/view?usp=share_link
Taktiež prikladáme zoznam súborov ktorý budete potrebovať pre vaše odpovede. V tomto súbore nájdete všetky súbory z /etc/ s príslušnými číslami. https://drive.google.com/file/d/1tmNtsSdnloLi-RyATmTMb_FKzd21Aiz1/view?usp=share_link <br/>
Reported Difficulty: 1

## 1 SSH
> Naša firemná politika nám káže, aby sa na server nedalo prihlásiť cez ssh ako root, a taktiež aby nedovoľovalo prihlásenie do servera cez ssh s prázdnym heslom. Ktoré riadky a súbory je potrebné zmeniť aby sme dodržali firemnú politiku?
Formát vlajky je file_number:line_number,file_number:line_number. Príklad: Pre riadky 11 a 14 v súbore systemd/sleep.conf a riadok 22 v súbore cloud/cloud.cfg použite formát 47:22,89:11,89:14. Zoraďte výsledky od najnižšieho po najvyšší (správne: 47:22,89:11,89:14, nesprávne: 89:11,89:14,47:22).

## 2 Apache2
> Ako webovú službu používame Apache2, je potrebné nastaviť aby sme pri vstupe na stránku na zložku, nevideli zoznam súborov ktoré obsahuje (napríklad, ale nie limitované na http://our_website.com/uploads/). Taktiež je potrebné nastaviť aby sa v prípade kompromitácie webový používateľ nedokázal prihlásiť ako root cez sudo bez hesla. Ktoré riadky a súbory je potrebné zmeniť?
Formát vlajky je file_number:line_number,file_number:line_number. Príklad: Pre riadky 11 a 14 v súbore systemd/sleep.conf a riadok 22 v súbore cloud/cloud.cfg použite formát 47:22,89:11,89:14. Zoraďte výsledky od najnižšieho po najvyšší (správne: 47:22,89:11,89:14, nesprávne: 89:11,89:14,47:22).

## 3 FTP
> Teraz potrebujeme zmeniť konfiguráciu nášho ftp, potrebujeme aby anonymní používatelia mohli nahrávať súbory do /var/www/html/uploads/, ale potrebujeme im zabrániť aby tam mohli vytvárať zložky alebo meniť a mazať subory. Ktoré riadky a súbory je potrebné zmeniť?
Formát vlajky je file_number:line_number,file_number:line_number. Príklad: Pre riadky 11 a 14 v súbore systemd/sleep.conf a riadok 22 v súbore cloud/cloud.cfg použite formát 47:22,89:11,89:14. Zoraďte výsledky od najnižšieho po najvyšší (správne: 47:22,89:11,89:14, nesprávne: 89:11,89:14,47:22).

## 4 Fail2Ban
> Aby sme sa zabezpečili proti bruteforce útokom, nainštalovali sme fail2ban, viete ho nakonfigurovať tak aby sa prístup na služby zablokoval po 6 pokusoch, pristup na vsftpd po 3 pokusoch a všeobecný bantime trval 30 minút? Ktoré riadky a súbory je potrebné zmeniť?
Formát vlajky je file_number:line_number,file_number:line_number. Príklad: Pre riadky 11 a 14 v súbore systemd/sleep.conf a riadok 22 v súbore cloud/cloud.cfg použite formát 47:22,89:11,89:14. Zoraďte výsledky od najnižšieho po najvyšší (správne: 47:22,89:11,89:14, nesprávne: 89:11,89:14,47:22).

## 5 Logrotate
> Teraz je potrebné nastaviť logrotate pre systémové logy tak, aby sa rotovali každý deň, a to do množstva 10. Taktiež je potrebné nastaviť logrotate pre fail2ban aby sa týždenne archivované logy udržiavali aspoň 12 týždňov. Ktoré riadky a súbory je potrebné zmeniť?
Formát vlajky je file_number:line_number,file_number:line_number. Príklad: Pre riadky 11 a 14 v súbore systemd/sleep.conf a riadok 22 v súbore cloud/cloud.cfg použite formát 47:22,89:11,89:14. Zoraďte výsledky od najnižšieho po najvyšší (správne: 47:22,89:11,89:14, nesprávne: 89:11,89:14,47:22).

