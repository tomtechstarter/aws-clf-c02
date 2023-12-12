# RDS Erstellen

## Datenbank - Subnetz Gruppe erstellen
1. Zu dem Service RDS navigieren 
2. In der Seitenleiste Subnetzgruppen auswählen 
3. Subnetzgruppe erstellen 
4. Wähle dein VPC aus 
5. Wähle mindestens 2 AZs aus 
6. Bei den Subnetzen wähle die ÖFFENTLICHEN Subnetze aus
   --> Du musst dir hierzu in einem neuem Fenster die IDs zu den öffentlichen Subnetzen unter dem Service VPC raussuchen 

## Neue MySQL Datenbank erstellen 
1. RDS aufrufen 
2. DB Instances aufrufen 
3. Datenbank erstellen
4. MYSQL auswählen 
5. Vorlage --> Kostenloses Kontingent
6. Passwort festlegen
7. Unter Instance-Konfiguration db.t3.micro auswählen
8. Unter Anbindung 
  --> Euer VPC auswählen
  --> Die Zuvor erstellte Subnetzgruppe auswählen
  --> Öffentlicher Zugriff: Ja
  --> Falls keine mysql-sg vorhanden, neue Sicherheitsgruppe erstellen
9. Datenbank erstellen
10. Warten bis die Datenbank bereit steht
11. Endpunkt in Zwischenablage kopieren 

## MySQL Workbench
1. Neue Verbindung über das + Erstellen 
2. Namen eingeben für die Verbindung z.B. aws-rds
3. unter Hostname den Endpunkt einfügen https://meet.google.com/omm-dusq-dvt
4. Benutzername zu admin ändern
5. Passwort eingeben
6. Verbindung sollte hergestellt sein
7. Bitte denkt daran die RDS wieder zu löschen 
 