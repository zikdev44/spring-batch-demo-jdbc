# spring-batch-demo-jdbc
Ce projet vise à démontrer une implémentation basique et extensible de Spring Batch pour le traitement de fichiers. Il permet de lire un fichier CSV contenant des données clients, de les transformer, puis de les insérer dans une base de données relationnelle.
Il est conçu pour être facile à comprendre, tout en permettant une montée en puissance rapide vers un système plus robuste et extensible.
# Lancement
Lancer le projet avec argument inputFile=C:\\dev\\dataBatch\\spring-batch\\InputFiles\\students.csv
# Procédure
1. Ouvre IntelliJ IDEA et accède à "Run → Edit Configurations".
2. Dans la section "Program arguments", ajoute l'argument suivant : inputFile=C:\dev\dataBatch\spring-batch\InputFiles\students.csv
3. Applique les modifications et exécute l'application.
# Script sql de la table student
```sql
CREATE TABLE `student` (
  `id` bigint(20) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(255) NOT NULL,
  `last_name` varchar(255) NOT NULL,
  `email` varchar(255) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `email` (`email`)
) ENGINE=InnoDB AUTO_INCREMENT=101 DEFAULT CHARSET=latin1;


