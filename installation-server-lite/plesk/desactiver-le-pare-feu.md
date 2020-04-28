---
description: Pour désactiver le pare feu de plesk
---

# Désactiver le pare feu

## Désactiver le pare feu sur le panel plesk

Le pare feu est souvent bien pratique mais il peut aussi poser quelques problèmes surtout avec les launcher

![cherchez le bouton concernant le pare feu](../../.gitbook/assets/unknown-1.png)

Vous arriverez sur un page comme ça:

![](../../.gitbook/assets/7ape0rj-1.png)

{% hint style="info" %}
Il y a plusieurs moyens de désactiver le pare feu. Préférez la première méthode à la seconde
{% endhint %}

#### Première méthode

La première méthode consiste à désactiver juste la partie du firewall \(la règle\) qui pose problème

![cliquez sur CWAF pour l&apos;envoyer dans l&apos;autre list puis cliquez sur valider](../../.gitbook/assets/bztqpff-1.png)

{% hint style="warning" %}
Chez moi c'est le CWAF qui pose problème mais si ça ne résous pas le problème chez vous, procédez par élimination jusqu’à trouver la règle récalcitrante
{% endhint %}

#### Seconde méthode

La seconde méthode consiste à désactiver l'entièreté du pare-feu

{% hint style="danger" %}
Attention cela peut rendre votre site plus vulnérable à des actes malveillants
{% endhint %}

![S&#xE9;lectionnez &quot;D&#xE9;tection uniquement&quot; puis cliquez sur OK](../../.gitbook/assets/gyaz9wf-1.png)

{% hint style="success" %}
Normalement tout devrait être réparé
{% endhint %}

