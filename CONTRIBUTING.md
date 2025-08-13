##CONTRIBUTING.md

Voici un modèle complet pour votre fichier **CONTRIBUTING.md** adapté à votre projet R-F Generator :

```markdown
# 🚀 Guide de Contribution

Nous sommes ravis que vous souhaitiez contribuer à R-F Generator ! Voici comment participer efficacement.

## 🌟 Premiers Pas

1. **Fork** le dépôt
2. **Clone** votre fork :
   ```bash
   git clone https://github.com/votre-username/R-F-generator.git
   ```
3. **Créez une branche** :
   ```bash
   git checkout -b feature/nom-de-votre-fonctionnalite
   ```

## 🛠 Workflow de Développement

### Rapporter un Bug
1. Vérifiez que le bug n'existe pas déjà dans [les Issues](https://github.com/rogergra/R-F-generator/issues)
2. Créez une nouvelle Issue avec :
   - Titre clair
   - Étapes pour reproduire
   - Comportement attendu vs actuel
   - Captures d'écran si possible

### Proposer une Amélioration
1. Ouvrez une Issue avec le label `enhancement`
2. Décrivez :
   - Le besoin métier
   - Votre solution proposée
   - Impacts techniques

### Soumettre du Code
1. Codez en suivant le style existant
2. Testez vos modifications
3. Soumettez une Pull Request (PR) avec :
   - Description claire
   - Référence à l'Issue liée
   - Captures d'écran si changement UI

## 📝 Standards de Code

### JavaScript
- Utilisez ES6+
- Commentaires JSDoc pour les fonctions complexes
- Validation des entrées utilisateur

```javascript
/**
 * Calcule la consommation électrique
 * @param {number} oldIndex - Ancien index
 * @param {number} newIndex - Nouvel index
 * @returns {number} Consommation en kWh
 */
function calculateConsumption(oldIndex, newIndex) {
  if (isNaN(oldIndex) || isNaN(newIndex)) {
    throw new Error('Les index doivent être des nombres');
  }
  return newIndex - oldIndex;
}
```

### HTML/CSS
- HTML sémantique
- CSS avec préfixes BEM
- Mobile-first

```html
<div class="invoice-card">
  <div class="invoice-card__header">
    <h3 class="invoice-card__title">Facture #123</h3>
  </div>
</div>
```

## 🧪 Tests

1. Vérifiez le bon fonctionnement :
   - Génération de PDF
   - Calculs automatiques
   - Responsive design

2. Testez sur au moins :
   - Chrome/Firefox
   - Mobile (simulateur accepté)

## 📌 Processus de Revue

1. Un mainteneur vous assignera un reviewer
2. Les PR nécessitent :
   - ✅ 2 approbations
   - ✅ Tests réussis
   - ✅ Aucun conflit

3. Les commentaires de review seront marqués avec :
   - `nit`: Petit changement optionnel
   - `blocker`: Doit être corrigé avant merge

## 🏷 Système d'Étiquettes

| Étiquette         | Description                          |
|-------------------|--------------------------------------|
| `bug`             | Problème à corriger                  |
| `enhancement`     | Nouvelle fonctionnalité              |
| `documentation`   | Amélioration de la docs              |
| `good first issue`| Idéal pour nouveaux contributeurs    |

## 💬 Communication

- Discussions techniques : Issues GitHub
- Questions rapides : [Discord du projet](lien-invit-discord)
- Respectez notre [Code de Conduite](CODE_OF_CONDUCT.md)

Merci pour votre contribution ! ⚡
```
