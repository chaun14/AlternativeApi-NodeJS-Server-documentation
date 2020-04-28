---
description: Installer le système sur un hébergement web cPanel
---

# cPanel

Connectez vous sur votre panel cPanel et allez sur la page principale

![Un exemple de cPanel](../.gitbook/assets/3c65oae-1.png)

## Préparation

{% hint style="info" %}
NodeJS monopolise le domaine qu'on lui donne, on ne peux pas mettre un site à coté,  donc je conseil de le placer dans un sous domaine comme je le fais dans ce tuto
{% endhint %}

Nous allons commencer par créer un sous domaine qui sera dédié au launcher   


![Cherchez un bouton pour ajouter un sous domaine si votre offre le permet](../.gitbook/assets/2hvi59z-1.png)

![Je l&apos;ai nomm&#xE9; launcher pour bien m&apos;y retrouver ce qui me donnera launcher.tuto.chaun14.fr](../.gitbook/assets/10dgvkn-1.png)

## Installation

Connectez vous en ftp à votre hébergement avec WinSCP ou FileZilla par exemple

Faites en sorte d'être à la racine de vote hébergement 

![Ne faites pas attention &#xE0; tous ce bazar](../.gitbook/assets/avegbze-1.png)

Créez un dossier nommé par exemple launcher. Cliquez dessus et diminuez la fenêtre de votre client ftp.

Nous allons maintenant télécharger le serveur NodeJS depuis github [ici](https://github.com/chaun14/AlternativeApi-NodeJS-Server-lite/archive/master.zip)

Une fois l'archive téléchargée, extrayez la sur votre pc et envoyez le contenu du dossier master vers le dossier files nouvellement créé

![](../.gitbook/assets/1shu1pb-1.png)

![Vous devez avoir quelque chose de ce genre](../.gitbook/assets/hma9opm-1.png)

{% hint style="info" %}
Vous pouvez supprimer les .bat qui ne servent que sous windows
{% endhint %}

## Lancement

Retournez maintenant sur le cPanel et cherchez le bouton `Setup NodeJS App` 

![](../.gitbook/assets/mkippwq-1.png)

Créez une nouvelle app

![](../.gitbook/assets/q92dmat-1.png)

Et remplissez les infos demandées

![](../.gitbook/assets/pqeygjw-1.png)

`Node.js version:` Fonctionne avec la V11.X et la V12.X  
`Application mode:` Choisissez Production  
`Application root:` chemin vers le dossier qui contient le serveur web NodeJS  
`Application URL:` choisissez votre sous domaine ou votre domaine si vous n'en avez pas la possibilité   
`Application statup file:` lien vers le fichier principal du serveur, ici `app.js`   
`Passenger log file:` choisissez ou les logs seront écrits 

Une fois ces information remplies cliquez sur `create app`

Si tout se passe bien vous devez arriver sur une page comme celle là

![](../.gitbook/assets/oeqyzxv-1.png)

Cliquez sur `run npm install` puis attendez quelques instants que tout s'installe.

![](../.gitbook/assets/4rlkxt6-1.png)

 Une fois que l'installation est terminée, cliquez sur le bouton `restart app` 

Rendez vous sur le sous domaine que vous avez créé et si vous voyez ça

![](../.gitbook/assets/6efowjo-1.png)

C'est que tout est installé correctement ✅  
Il ne vous reste plus qu'a coller le lien de votre sous domaine dans le launcher

{% hint style="info" %}
En cas de problèmes, n'hésitez pas à demander de l'aide sur le serveur discord de AlternativeAPI   
Lien: [https://discord.gg/8suwuu](https://discord.gg/8suwuu)
{% endhint %}

