# Le Mouchard

Qui te suit vraiment sur Instagram — sans mot de passe.

Le Mouchard lit l'export officiel de tes données Instagram (format JSON) directement dans ton navigateur. Aucun login, aucune requête vers Instagram, aucun serveur : tout reste sur ton téléphone.

- **Un export** : qui ne te suit pas en retour, comptes fantômes, totaux.
- **Deux exports** : qui t'a unfollow, qui t'a suivi, qui tu as quitté, évolution nette.

## Installer sur ton téléphone

Ouvre l'app depuis GitHub Pages, puis :

- **iPhone (Safari)** : bouton Partager → *Sur l'écran d'accueil*.
- **Android (Chrome)** : menu ⋮ → *Installer l'application*.

L'app fonctionne ensuite hors ligne.

## Développement

Site statique, aucun build : `index.html`, `manifest.webmanifest`, `sw.js`, `icons/`.

```bash
python3 -m http.server 8000
```

Après une modification, change `VERSION` dans `sw.js` pour que les téléphones récupèrent la nouvelle version.
