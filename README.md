# policlinica-cu-baza-de-date
Acest proiect reprezintă un sistem de management pentru o policlinică, implementat în Java și utilizând o bază de date pentru gestionarea informațiilor despre utilizatori, programări și consultații.

Funcționalități principale

Pacienți
Pot crea un cont și se pot autentifica.
Pot efectua programări la medici.

Angajați
Pot vizualiza și valida programările pacienților.

Medici
Pot efectua consultații.
Pot adăuga parafa pe consultațiile efectuate.

Admin
Poate adăuga, edita și șterge date despre angajați.

Super Admin
Are aceleași drepturi ca Admin, dar poate și gestiona conturile de Admin.

Tehnologii utilizate
Java – Limbaj principal pentru dezvoltarea aplicației.
MySQL/PostgreSQL – Baza de date utilizată pentru stocarea informațiilor.
JavaFX/Swing – Dacă aplicația are o interfață grafică.

Structura Proiectului

proiect-policlinica/
│-- src/
│   ├── main/java/com/policlinica/
│   │   ├── controllers/   # Logica aplicației
│   │   ├── models/        # Clasele entităților
│   │   ├── services/      # Servicii pentru interacțiunea cu baza de date
│   │   ├── repositories/  # Interfațe pentru accesarea bazei de date
│   │   ├── utils/         # Utilitare și configurări
│   ├── resources/
│       ├── application.properties  # Configurare BD
│       ├── schema.sql  # Script pentru baza de date
│-- pom.xml (dacă se folosește Maven)
│-- README.md


Autentificare și Role Management

Sistemul utilizează autentificare pe bază de roluri:

Pacient (ROLE_PATIENT)
Angajat (ROLE_EMPLOYEE)
Medic (ROLE_DOCTOR)
Admin (ROLE_ADMIN)
Super Admin (ROLE_SUPER_ADMIN)
