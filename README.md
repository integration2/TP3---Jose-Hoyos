# Autoévaluation

**TP3 - Intégration d'un formulaire accessible**

Compléter cette autoévaluation au fur et à la mesure. Seul les critères HTML devraient être complétés pour la remise d'étape 1.

---

**Barème :**
A = 100 % (tous les sous-critères respectés, réussite complète)
B = 85 % (presque tous les critères respectés)
C = 75 % (quelques lacunes)
D = 65 % (atteinte minimale du critère)
E = 55 % (lacunes majeures)

---

## Critères

### HTML (5 points)

- [x] **Balises structurelles et sémantiques** — Page avec `header`, `main`, `footer`. Bon choix du type d'input (ex. `type="email"` pour le courriel).
- [ ] **Code HTML valide** — Capture d'écran avant/après ou juste après validation pour prouver qu'il n'y a aucune erreur (les avertissements ne comptent pas).
- [x] **Regroupements et étiquetage** — `fieldset` pour grouper, `legend` pour étiqueter. `label` relié au `input` par `for`/`id`. Images avec `alt` documenté.
- [ ] **Contraintes de saisie** — Utilisation de `required`, `pattern` et `title`.
- [ ] **Conteneurs de validation** — Prévoir des balises `p.erreur` pour recevoir les messages d'erreur ou d'encouragement de la validation JavaScript. Ces balises doivent avoir un parent ou ancêtre commun (avec la classe `.ctnValidation`) avec l'élément ou les éléments de formulaire à valider.

Exemple pour le cas d'un seul élément :

```html
  <form action="index.html" method="get" class="formulaire">

            <fieldset id="format-brochure" class="section-formulaire">
            <div class="separateur"></div>
    
                <legend id="format-brochure__titre" class="section-brochure__titre">
                    <img class="image__titre" src="images/icon-format-brochure.svg">
                    <p>Format de la brochure</p>
                </legend>
                <ul class="format-brochure__liste">
                    <li class="format-brochure__liste-element">
                        <input type="radio" name="format-brochure__type" id="format-brochure__imprime" value="imprime" class="screen-reader-only">
                        <img class="image__format-brochure" src="images/icon-file-print.svg">
                        <label for="format-brochure__imprime" class="format-brochure__label">Imprimé</label>
                    </li>
                    <li class="format-brochure__liste-element">
                        <input type="radio" name="format-brochure__type" id="format-brochure__pdf" value="pdf" class="screen-reader-only">
                        <img class="image__format-brochure" src="images/icon-file-pdf.svg">
                        <label for="format-brochure__pdf" class="format-brochure__label">PDF</label>
                    </li>
                    <li class="format-brochure__liste-element">
                        <input type="radio" name="format-brochure__type" id="format-brochure__epub" value="epub" class="screen-reader-only">
                        <img class="image__format-brochure" src="images/icon-file-epub.svg">
                        <label for="format-brochure__epub" class="format-brochure__label">ePub</label>
                    </li>
                </ul>
                
            </fieldset>
```

#### Ma note d'autoévaluation pour le critère HTML : C

### CSS (6 points)

- [x] **Mobile first** — Règles pour l'écran étroit écrites en premier ; requêtes média imbriquées pour obtenir tout de suite après dans la CSS les variantes pour l'écran large.
- [x] **Styles de base** — Champs de saisie alignés. La variante pour l'écran large doit être enrichie par rapport à la version de l'écran étroit.
- [x] **Variables CSS** — Au moins deux variables CSS utilisées pour les couleurs.
- [x] **Documentation** — Commentaires dans la CSS et table des matières maintenue en tête de fichier.
- [ ] **Interactivité** — Lorsqu'un élément de formulaire reçoit le focus, son apparence doit changer pour le mettre en évidence. Le bouton de soumission et les hyperliens doivent avoir des états survol.
- [x] **Boutons radio** — Boutons radio visuellement cachés mais accessibles. Ce sont leurs étiquettes qui affichent les états normal, focus, hover et checked.

#### Ma note d'autoévaluation pour le critère CSS : B

### Accessibilité (4 points)

- [x] **Navigation au clavier** — Tab parcourt le formulaire dans le bon ordre. Enter soumet le formulaire.
- [ ] **Lien « Allez au contenu »** — Lien tout de suite après l'ouverture du `body`, permettant d'aller directement au contenu principal. Classes `screen-reader-only` et `focusable`.
- [ ] **Régions (landmarks)** — Utiliser les éléments HTML appropriés (`header`, `main`, `footer`) ou, si ce n'est pas possible, leur attribuer les rôles ARIA correspondants (`banner`, `main`, `contentinfo`).
- [ ] **Contraste des couleurs** — Changez les couleurs de bases fournies dans la maquettes pour des couleurs personnalisées et ajoutez, en commentaire de la feuille de styles, le niveau de contraste entre les couleurs utilisées et les tests réussis avec l'outil [TPGi Color Contrast Checker](https://www.tpgi.com/color-contrast-checker/).

#### Ma note d'autoévaluation pour le critère Accessibilité : D

### JavaScript (sera évalué dans le cours de programmation)

- [ ] Vérifier que les champs de saisie ne sont pas vides ; afficher un message d'erreur
- [ ] Vérifier que les données sont conformes au type attendu ; afficher un message d'erreur

#### Ma note d'autoévaluation pour le critère JavaScript : Z

---

**TOTAL**
X sur 15

---

## Ajoutez vos commentaires sur le projet. Comment ça s'est passé? Quels aspects avez-vous trouvé facile ou difficile?

J'ai eu de la difficulté avec la fin de ce projet, j'ai oublié d'enregistrer mon projet et j'ai perdu la plupart de mon progrès final, mais je suis fier de mon utilisation de flexbbox qui s'est amélioré, c'était un de mes objectifs durant le premier TP et je suis fier de l'Avoir réussi.

## Ma note d'autoévaluation pour le projet entier : C

capture d'écran : [capture-d'ecran](images/screencapture-integration2-github-io-tp1-JosemHoyos-2026-04-02-07_27_14.png)
