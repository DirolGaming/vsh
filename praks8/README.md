#### Nimelahenduste loomine
1. Panin apache ja db masinad käima
2. Lisasin /etc/hosts faili kirjed:

10.0.2.5 wp.jaagop.ee

10.0.2.5 wiki.jaagop.ee

3. Kopeerisin 000-default conf faili kaks korda ja seadistasin nende nimed:

wp.jaagop.ee.conf

wiki.jaagop.conf

4. Muutsin vastavalt conf failile ServerName ja Aliase koos DocumentRootiga ära
5. Tõstsin vastava sisuga wiki ja wordpress failid /var/www/html/wiki ja /var/www/html/wp/
6. Viisin läbi käsud a2ensite wiki.jaagop.ee ja a2ensite wp.jaagop.ee
7. Testisin asja Ubuntu kliendi peal kõike ja külastasin lehekülgi.
8. The end.


