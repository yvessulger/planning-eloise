# Jarvis Briefing

Briefing quotidien généré chaque matin vers 05h30 (heure suisse) par une tâche planifiée Claude.

| Fichier | Rôle |
|---|---|
| `dashboard.html` | Source du tableau de bord (publié comme artifact privé sur claude.ai) |
| `latest.txt` | Texte du briefing audio du jour, lu par le raccourci iPhone |

Ce dépôt est **public** : `latest.txt` ne contient que de l'actualité, sans donnée personnelle.

URL lue par le raccourci :

```
https://raw.githubusercontent.com/yvessulger/planning-eloise/jarvis/jarvis-briefing/latest.txt
```

## Raccourci iPhone « réveil → briefing → Thunderstruck »

### 1. Installer une bonne voix (une seule fois)
Réglages → Accessibilité → Contenu énoncé → Voix → Français → télécharge une voix masculine en qualité **Améliorée** ou **Premium**.
Les intitulés exacts peuvent varier selon la version d'iOS.

### 2. Créer le raccourci
App **Raccourcis** → onglet **Raccourcis** → **+** → nomme-le « Briefing Jarvis ». Ajoute dans l'ordre :

1. **Régler le volume** → 60 %
2. **URL** → colle l'URL ci-dessus
3. **Obtenir le contenu de l'URL**
4. **Énoncer le texte** → entrée : *Contenu de l'URL*. Touche la flèche pour afficher les options : **Attendre la fin** activé, **Langue** Français, **Voix** celle téléchargée, débit selon ton goût.
5. Musique, au choix :
   - **Apple Music** : action **Lire la musique** → choisis *Thunderstruck* (le titre doit être dans ta bibliothèque).
   - **Spotify** : dans Spotify, ouvre *Thunderstruck* → Partager → Copier le lien. Dans Raccourcis, ajoute **Ouvrir l'URL** avec ce lien. La lecture automatique n'est pas garantie : il faudra peut-être toucher Lecture.

Teste-le une fois en touchant ▶.

### 3. Le déclencher au réveil
Onglet **Automatisation** → **+** → **Alarme** → **Est arrêtée** → choisis ton alarme de réveil (ou « Tout réveil ») → **Exécuter immédiatement** → sélectionne le raccourci « Briefing Jarvis ».

Teste un matin avec le téléphone verrouillé : selon la version d'iOS, certaines actions demandent un déverrouillage.

## Si le briefing n'est pas à jour
La première ligne du texte annonce la date. Si elle n'est pas celle du jour, la tâche de 05h30 a échoué : le tableau de bord sur claude.ai indique le dernier briefing disponible.
