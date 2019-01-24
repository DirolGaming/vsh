### Praktikum 4 - SSL sertifikaadi tegemine IP-le

1. Viisin läbi käsu: sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/ssl/private/apache-selfsigned.key -out /etc/ssl/certs/apache-selfsigned.crt
2. Sisestasin vastava info (Country Name, State, Locality Name, Organization Name, Organizational Unit name, Common name [siia lisasin serveri IP], Email Address);
3. Viisin läbi käsu: sudo openssl dhparam -out /etc/ssl/certs/dhparam.pem 2048
4. Viisin läbi käsu: sudo nano /etc/apache2/conf-available/ssl-params.conf
5. Muutsin faili sisu (ssl-params.conf fail on ka siia lisatud)
6. Muutsin default-ssl.conf sisu lisades juurde Servername 172.23.13.51, muutes ära SSLCertificateFile and SSLCertificateKeyFile apache-selfsigned.crt ja ._.key peale
7. Lisasin 000-default.conf faili Redirect reegli- Redirect "/" "https://172.23.13.51"
8. aktiveerisin kõik seaded: sudo a2enmod ssl
sudo a2enmod headers sudo a2ensite default-ssl sudo a2enconf ssl-params
9. Taaskäivitasin Apache sudo systemctl restart apache2
10. Tehtud
