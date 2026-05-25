```markdown
# 016 — FreeTube

- **Source** : [GitHub - FreeTubeApp/FreeTube](http://github.com/FreeTubeApp/FreeTube)
- **Catégorie** : Médias
- **Langage** : JavaScript (Electron)
- **Licence** : GPL-3.0
- **Date** : 2026-05-25

## Ce que c'est
FreeTube est un client desktop pour YouTube qui respecte la vie privée. Il permet de regarder des vidéos sans publicités, sans suivi (tracking) et sans nécessiter de compte Google.

## Fonctionnement
- **Interface locale** : Fonctionne hors navigateur, sans dépendre des services Google.
- **Intégration API** : Utilise des proxys comme Invidious ou Piped pour récupérer les vidéos.
- **Personnalisation** : Permet de bloquer les recommandations, désactiver les miniatures, etc.
- **Multiplateforme** : Disponible pour Windows, macOS et Linux.
- **Open Source** : Code source accessible et modifiable.

## Cas d'usage typique
- Regarder des vidéos YouTube sans être suivi par Google.
- Éviter les publicités intrusives lors de la lecture.
- Utiliser YouTube en mode hors ligne ou avec une meilleure gestion des abonnements.

## Installation rapide
```bash
# Via Flatpak (recommandé)
flatpak install flathub io.freetubeapp.FreeTube

# Via Snap
sudo snap install freetube

# Via AppImage (téléchargement manuel)
wget https://github.com/FreeTubeApp/FreeTube/releases/latest/download/FreeTube-*.AppImage
chmod +x FreeTube-*.AppImage
./FreeTube-*.AppImage
```

## Pourquoi le retenir
FreeTube est une alternative éthique à l'application officielle YouTube, idéale pour les utilisateurs soucieux de leur vie privée et souhaitant éviter le tracking omniprésent de Google.
```