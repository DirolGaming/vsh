#### DokuWiki paigaldamine Apache2 ja Debianile

1. Tegin uue kausta asukohas /var/www/html/ nimega wiki
2. Sisenesin sinna kausta cd /var/www/html/wiki
3. Tõmbasin alla dokuwiki tar faili (wget http://download.dokuwiki.org/src/dokuwiki/dokuwiki-stable.tgz
4. Avasin paki tar xvf dokuwiki-stable.tgz
5. Muutsin kausta õigused sudo chmod -R 707 /var/www/html/wiki/
6. Külastasin lehte 10.0.2.5/wiki ja tuli ette Dokuwiki lehe loomise tekst

* Seda saab ka lihtsamalt, aga kuna Dokuwiki pidevalt ulgus oma neetud õiguste üle (/usr/share/dokuwiki/) isegi kui www-data oli kausta ja failide omanik, otsustasin teha asja lihtsama vastupanu teed.

