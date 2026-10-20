# Le Mouchard

Mon tableau de bord Instagram perso : qui m'a unfollow, qui m'a suivi, qui ne me suit pas en retour — sans mot de passe.

L'app lit l'export officiel de tes données Instagram (format JSON) directement dans le navigateur. Aucun login, aucune requête vers Instagram, aucun serveur : tout reste sur le téléphone.

## Utilisation

1. **Ajouter** : choisis le .zip de l'export Instagram (ou les fichiers .json). Le dernier export est mémorisé, il suffit ensuite d'ajouter le nouveau. Le .zip est lu dans le navigateur, rien n'est envoyé.
2. **Accueil** : abonnés, évolution, partis / arrivés, sans retour, fantômes, faux départs (pseudos changés, comptes disparus ou revenus), historique.
3. **Explorer** : croissance depuis le début, réciprocité, relations (demandes en attente, tes unfollows, amis proches), activité (J'aime, commentaires, stories, enregistrements, recherches), messages, infos du compte.

## Installer sur le téléphone

- **iPhone (Safari)** : Partager → *Sur l'écran d'accueil*.
- **Android (Chrome)** : menu ⋮ → *Installer l'application*.

## Développement

Site statique, aucun build : `index.html`, `manifest.webmanifest`, `sw.js`, `icons/`.

```bash
python3 -m http.server 8000
```

Après une modification, change `VERSION` dans `sw.js` pour que le téléphone récupère la nouvelle version.
