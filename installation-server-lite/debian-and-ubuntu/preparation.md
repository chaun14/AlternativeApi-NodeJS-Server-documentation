---
description: les dépendances
---

# Préparation

## Préparation, les dépendances

Pour commencer, vérifiez que votre systèmes est bien à jour avec cette commande:

```text
sudo apt install && apt upgrade
```

Pour fonctionner, le serveur a besoin de NodeJS.

{% hint style="danger" %}
Si vous faites directement `apt install nodejs` nous aurez une version obsolète de node qui ne pourra pas faire démarrer 
{% endhint %}

Pour éviter cela nous devons effectuer ces commandes afin d'installer NodeJS v12

```text
sudo apt -y install curl
sudo curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt -y install nodejs
```

Désormais si vous faites `node -v` vous devez obtenir quelque chose comme `v12.16.3`

{% hint style="success" %}
L'installation des dépendances est terminée
{% endhint %}

