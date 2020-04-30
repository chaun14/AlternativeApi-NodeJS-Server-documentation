---
description: >-
  Lancer le serveur en arrière plan pour le laisser allumer même quand vous
  n'êtes plus sur le teminal.
---

# Faire tourner en arrière plan

Il y a plusieurs moyens de faire ça 

## Avec forever

Effectuez la commande pour installer forever sur tout le système

```text
npm i -g forever
```

Ensuite faites 

```bash
forever start app.js
```

et le système tournera en arrière plan et redémarrera en cas de crash du processustu nodejs

{% hint style="warning" %}
En cas de redémarrage du vps vous devrez retourner dans le répertoire du serveur \(`cd /var/www/launcher-lite`\) et refaire la commande si dessus
{% endhint %}

## Avec systemd

Bientôt...



