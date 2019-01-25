#### Praktikum 6 - Wordpress kaug andmebaasiserveriga

1. Installeerisin Wordpressi esimesele masinale peale koos LAMP stackiga (sama mis praktikum5-s põhimõtteliselt).
2. Installeerisin teise masina peale MySQL andmebaasi (sudo apt install mysql-server)
2.1 Tasub mainimist, et vahetasin hiljem MySQL MariaDB peale ümber, kuna see on stabiilsem ja kiirem kaugühenduste jaoks.
3. Lõin MariaDB-s andmebaasi nimega hello ja andsin kasutajale@10.0.2.5(wordpress serveri IP)-le kõik õigused.
4. Muutsin ära my.cnf bind addressi, asendasin selle serveri IP-ga (selle IP-ga kus mariadb jookseb)
5. Ühendasin ubuntu desktop-iga wordpressi lehele.
6. Seadistasin andmebaasi paroolid, hosti ja kasutajanime
7. Tehtud

* Lisan, et täpsed käsud on praktikum 5 README.md failis.
