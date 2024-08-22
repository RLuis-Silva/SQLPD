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
<br>
### Caso 5
"una lista di email di un servizio online illegale è stata inviata al SQLPD. Invia tutti i dettagli delle date di iscrizione. Assicurati che non ci siano duplicati."

SELECT DISTINCT JoinDate
FROM mailing_list;
<br>
### Caso 6
"un hacker ha inviato al SQLPD i dettagli degli abbonamenti esposti di un sito losco collegato a varie persone ricercate. Invia tutti i dettagli degli abbonamenti ordinati in base al numero di acquisti in ordine crescente."

SELECT *
FROM subscribers
ORDER BY NumberOfPurchases ASC;
<br>
### Caso 7
"i dettagli degli abbonamenti di un sito hackerato sono emersi su un forum darknet. invia tutti i dettagli abbonati ordinati per nome completo in ordine decrescente."

SELECT * 
FROM subscribers
ORDER BY FullName DESC;
<br>
### Caso 8
"i server di un sito illegale sono stati sequestrati in una recente operazione. Invia tutti gli indirizzi email degli utenti e i dettagli del numero di post ordinati per numero di post in ordine decrescente. Assicurati che non ci siano duplicati."

SELECT DISTINCT Emails, NumberOfPosts
FROM users
ORDER BY NumberOfPosts DESC;
<br>
### Caso 9
"una lista di email di un servizio online illegale è stata inviata al SQLPD. Invia tutti i numero di figli, i cognomi e i dettagli delle date di iscrizione ordinati per cognomi in ordine crescente e poi per numero di figli in ordine crescente."

SELECT NumberOfKids, FamilyName, Joined
FROM mailing_list
ORDER BY FamilyName ASC, NumberOfKids ASC;
<br>
### Caso 10
"una lista di emaul di un servizio online illegale è stata inviata al SQLPD. Invia i dettagli dei primi 3 records ordinati per cognome in ordine decrescente e poi per nome in ordine crescente."

SELECT *
FROM mailing_list
ORDER BY LastName DESC, FirstName ASC
LIMIT 3;
<br>
