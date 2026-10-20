# Le Mouchard

Mon tableau de bord Instagram perso : qui m'a unfollow, qui m'a suivi, qui ne me suit pas en retour — sans mot de passe.

L'app lit l'export officiel de tes données Instagram (format JSON) directement dans le navigateur. Aucun login, aucune requête vers Instagram, aucun serveur : tout reste sur le téléphone.

## Utilisation

1. **Ajouter** : la première fois, un ancien export et un récent. Ensuite le dernier est mémorisé, il suffit d'ajouter le nouveau.
2. **Accueil** : abonnés, évolution, partis / arrivés, sans retour, fantômes, historique des exports.
3. **Guide** : comment demander l'export à Instagram.

## Installer sur le téléphone

- **iPhone (Safari)** : Partager → *Sur l'écran d'accueil*.
- **Android (Chrome)** : menu ⋮ → *Installer l'application*.

## Développement

Site statique, aucun build : `index.html`, `manifest.webmanifest`, `sw.js`, `icons/`.

```bash
python3 -m http.server 8000
```

Après une modification, change `VERSION` dans `sw.js` pour que le téléphone récupère la nouvelle version.
