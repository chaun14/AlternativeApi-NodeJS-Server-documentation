---
description: Déployez le serveur NodeJS lite sur votre vps
---

# Installation

Personnellement j'aime bien installer mes serveur web ici dans ce répertoire `/var/www/` mais vous pouvez le mettre ou vous voulez, il faudra juste

Pour commencer nous allons créer le répertoire qui va accueillir notre serveur 

```text
cd /var/www/
mkdir launcher-lite
cd launcher-lite
```

Nous allons télécharger le serveur nodejs 

```text
wget https://codeload.github.com/chaun14/AlternativeApi-NodeJS-Server-lite/zip/master
```

Maintenant nous allons extraire le serveur

```text
unzip master
cd AlternativeApi-NodeJS-Server-lite-master
mv * ../
rm -rf AlternativeApi-NodeJS-Server-lite-master
rm master
```

