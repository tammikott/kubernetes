# Kubernetes k3s Labor

Selle labori raames paigaldasin ja konfigureerisin k3s Kubernetes klaster Ubuntu 22.04 masinale.

## Tehtud tööd

### 1. k3s Paigaldus
- Installisin k3s single-node klaster
- Konfigureerisin kubectl kasutamiseks
- Kontrollisin klasteri olekut

### 2. Podide Loomine
- Lõin nginx Podi käsurea abil (`kubectl run`)
- Lõin nginx Podi YAML faili abil
- Testisin Podi tööd sisse logimise ja logide vaatamisega

### 3. Deploymentide Kasutamine
- Lõin nginx Deploymenti 3 koopiaga
- Testisin self-healing funktsiooni (Pod kustutamine → automaatne taastamine)
- Skaleerisin Deploymentit (2 → 5 → 2 koopiat)
- Tegin rolling update nginx 1.25 → 1.26
- Testisin rollback funktsiooni

### 4. Service'ide Konfigureerimine
- Lõin ClusterIP Service'i sisevõrgu jaoks
- Lõin NodePort Service'i välistele päringutele
- Testisin Service'i tööd DNS nime kaudu
- Kontrollisin Endpoint'ide õiget seostamist

### 5. PostgreSQL Rakendus
- Lõin Secreti parooli hoidmiseks
- Lõin PostgreSQL Deploymenti ja Service'i
- Testisin andmebaasi ühendust Service'i kaudu
- Kontrollisin Secreti õiget kasutamist

### 6. Ressurside Puhastamine
- Kustutasin kõik loodud ressursid
- Kontrollisin, et klaster on puhas

## Kasutatud Tehnoloogiad
- **k3s** - Lightweight Kubernetes
- **Docker** - Container runtime
- **kubectl** - Kubernetes CLI
- **YAML** - Konfiguratsioonifailid
- **PostgreSQL** - Andmebaas
- **nginx** - Web server

## Failide Struktuur
