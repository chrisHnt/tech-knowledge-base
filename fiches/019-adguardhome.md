# 019 — AdGuard Home

- **Source** : [GitHub - AdguardTeam/AdGuardHome](http://github.com/AdguardTeam/AdGuardHome)
- **Catégorie** : Réseau
- **Langage** : Go
- **Licence** : GPL-3.0
- **Date** : 2026-05-25

## Ce que c'est
AdGuard Home est un bloqueur de publicités et de trackers au niveau du réseau, conçu pour protéger tous les appareils connectés à votre domicile (y compris les smart TVs, smartphones, tablettes, etc.). Contrairement aux solutions locales comme Pi-hole, il fonctionne comme un serveur DNS avec une interface web avancée pour une gestion centralisée.

## Fonctionnement
- **Serveur DNS intégré** : Remplace votre DNS existant (ex: celui de votre FAI) pour filtrer les requêtes malveillantes ou publicitaires.
- **Interface web intuitive** : Configuration, statistiques et gestion des règles via un tableau de bord accessible depuis n'importe quel navigateur.
- **Filtrage avancé** : Utilise des listes de blocage personnalisables (ex: EasyList, EasyPrivacy) et permet d'ajouter des règles DNS personnalisées.
- **Protection multi-appareils** : Applique les règles à tous les appareils du réseau sans installation locale.
- **Chiffrement DNS** : Prend en charge DoH (DNS over HTTPS), DoT (DNS over TLS) et DNSCrypt pour une sécurité renforcée.

## Cas d'usage typique
- **Bloquer les publicités et trackers** sur tous les appareils de votre réseau domestique sans configuration individuelle.
- **Protéger les enfants** en filtrant les contenus inappropriés via des listes de blocage dédiées.
- **Améliorer la confidentialité** en évitant que les requêtes DNS ne soient interceptées par des tiers (FAI, annonceurs).

## Installation rapide
```bash
docker run --name adguardhome \
  -v /path/to/adguard/work:/opt/adguardhome/work \
  -v /path/to/adguard/conf:/opt/adguardhome/conf \
  -p 53:53/tcp -p 53:53/udp \
  -p 80:80/tcp -p 443:443/tcp \
  -p 3000:3000/tcp \
  --restart unless-stopped \
  adguard/adguardhome
```
Accédez ensuite à l'interface web via `http://<votre-ip>:3000` pour finaliser la configuration.

## Pourquoi le retenir
AdGuard Home est une solution **tout-en-un** pour un réseau sans publicités et plus sécurisé, avec une interface moderne et une flexibilité inégalée (filtrage personnalisable, chiffrement DNS, etc.). Idéal pour remplacer les solutions basiques comme Pi-hole lorsque vous avez besoin de plus de contrôle.