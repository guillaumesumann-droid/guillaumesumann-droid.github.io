# Guillaume Sumann — CV Radioprotection

Portfolio personnel de Guillaume Sumann, Ingénieur Radioprotection.  
**URL de production :** https://guillaumesumann-droid.github.io

---

## Déploiement sur GitHub Pages

### Prérequis
- Dépôt GitHub nommé exactement `guillaumesumann-droid.github.io`
- Le dépôt doit être **public**

### Fichiers du projet

```
guillaumesumann-droid.github.io/
├── index.html              ← site complet (CSS + JS inline)
├── photo-congres.jpg.JPG   ← photo AFTMN Nantes 2017
├── logo-dose-matin.png.PNG ← logo La Dose du Matin
└── README.md
```

> **Note images :** les fichiers images ont une double extension (`.jpg.JPG`, `.png.PNG`).
> Ils sont référencés tel quels dans le HTML. Pour éviter tout problème,
> vous pouvez les renommer en `.jpg` / `.png` et mettre à jour les deux
> attributs `src` correspondants dans `index.html`.

### Étapes de déploiement

1. **Initialiser le dépôt local** (si pas encore fait) :
   ```bash
   git init
   git remote add origin https://github.com/guillaumesumann-droid/guillaumesumann-droid.github.io.git
   ```

2. **Ajouter et committer les fichiers** :
   ```bash
   git add index.html README.md photo-congres.jpg.JPG logo-dose-matin.png.PNG
   git commit -m "Initial CV site"
   ```

3. **Pousser sur la branche principale** :
   ```bash
   git push -u origin main
   ```
   *(ou `master` selon la configuration de votre dépôt)*

4. **Activer GitHub Pages** :
   - Aller dans `Settings` → `Pages`
   - Source : **Deploy from a branch**
   - Branch : `main` (ou `master`), dossier `/ (root)`
   - Cliquer **Save**

5. **Attendre ~1 minute** puis visiter :  
   👉 https://guillaumesumann-droid.github.io

### Test local

Double-cliquer sur `index.html` — s'ouvre directement dans le navigateur, aucune dépendance serveur.

---

## Fonctionnalités

| Fonctionnalité | Détail |
|---|---|
| Mode clair / sombre | Bouton toggle en haut à droite, préférence sauvegardée |
| Typewriter hero | 4 phrases en rotation, animation fluide |
| Modales compétences | 6 domaines cliquables avec détails |
| Timeline horizontale | Scroll souris + glisser-déposer + tactile |
| Animations scroll | Fade-up au défilement via IntersectionObserver |
| Easter egg | Cliquer 3× sur le `·` du footer en moins de 2 secondes |
| Responsive | Mobile, tablette, desktop |

---

*Site statique — aucun build, aucune dépendance serveur. Fonctionne hors-ligne.*
