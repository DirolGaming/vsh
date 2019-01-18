### Apache 2 Veebiserveri paigaldamine

1. Paigaldamiseks viisin läbi käsu *apt install apache2*
2. Default lehe muutmiseks läksin asukohta /var/www/html/
3. Seal oli fail nimega "index.html"
4. Eemaldasin selle faili ja lõin uue sisuga:
<!DOCTYPE html>
<html>
<head>
<title>Jaagop Janson</title>
</head>
<body

<h1>ISP 117</h1>

<p>jaagop.janson@khkee</p>

</body>

</html>

(fail lisatud ka GitHub praks2 reposse)


5. public directory lisasin /var/www/html kausta juurde
6. Nüüd on ka ligipääsetav see 172.23.13.51/public
7. The end
