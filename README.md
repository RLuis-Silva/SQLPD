# SQLPD
riprendo SQL giocando a SQLPD (https://sqlpd.com/)

### Caso 1 
"una lista di email di un servizio online illegale è stata inviata alla SQLPD. Si prega di inviare i dettagli di tutte le voci."

  SELECT * 
  FROM mailing_list;
<br>
### Caso 2 
"un hacker ha inviato al SQLPD i dettagli dei membri di un sito losco collegato a varie persone di interesse. Invia i dettagli di tutti i membri."
 
  SELECT *
  FROM members;
<br>
### Caso 3 
"i server di un sito illegale sono stati sequestrati in una recente operazione. Invia le email di tutti gli utenti, gli ultimi orari di accesso e i dettagli dei cognomi."

SELECT Email, LastAccess, FamilyName
FROM users;
<br>
### Caso 4
"i dettagli dei membri di un sito hackerato sono emersi su un forum darknet. Invia i nomi completi e gli indirizzi postali di tutti i membri."

SELECT FullName, MailingAddress
FROM members;


