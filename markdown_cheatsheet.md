---
title = Markdown Datasheet
nav_order: 2
---

# Aide-mémoire Markdown

## Titres

```markdown
# Titre niveau 1 (le plus grand)
## Titre niveau 2
### Titre niveau 3
#### Titre niveau 4
```

## Formatage de texte

```markdown
**Texte en gras**
*Texte en italique*
***Gras et italique***
~~Texte barré~~
`code inline`
```

## Listes

### Liste à puces
```markdown
- Item 1
- Item 2
  - Sous-item 2.1
  - Sous-item 2.2
- Item 3
```

### Liste numérotée
```markdown
1. Premier
2. Deuxième
3. Troisième
```

### Liste de tâches
```markdown
- [x] Tâche terminée
- [ ] Tâche en cours
- [ ] Tâche à faire
```

## Liens et images

```markdown
[Texte du lien](https://url.com)
![Texte alternatif de l'image](chemin/image.png)
```

## Blocs de code

### Code inline
```markdown
Utilisez la commande `ls -la` pour lister les fichiers.
```

### Bloc de code avec syntaxe
````markdown
```bash
#!/bin/bash
echo "Hello World"
```

```python
def hello():
    print("Hello World")
```
````

## Citations

```markdown
> Ceci est une citation
> sur plusieurs lignes
```

## Séparateurs

```markdown
---
ou
***
ou
___
```

## Tableaux

```markdown
| Colonne 1 | Colonne 2 | Colonne 3 |
|-----------|-----------|-----------|
| Ligne 1   | Donnée    | Donnée    |
| Ligne 2   | Donnée    | Donnée    |
```

## Échappement de caractères

```markdown
\* Ceci n'est pas en italique \*
\# Ceci n'est pas un titre
```

Utilisez `\` avant un caractère spécial pour l'afficher littéralement.

## Liens internes (ancres)

```markdown
## Section 1 {#section1}

Retour à [Section 1](#section1)
```

## Notes de bas de page

```markdown
Texte avec une référence[^1]

[^1]: Ceci est la note de bas de page
```

## Émojis (si supportés)

```markdown
:smile: :rocket: :thumbsup:
```

Ou directement : 😊 🚀 👍

## HTML dans Markdown

Markdown accepte du HTML :

```html
<div style="color: red;">
Texte en rouge
</div>

<details>
<summary>Cliquez pour déplier</summary>
Contenu caché
</details>
```

## Conseils

1. **Ligne vide** = nouveau paragraphe
2. **Deux espaces en fin de ligne** = retour à la ligne sans nouveau paragraphe
3. **Indentation de 2-4 espaces** = sous-niveau dans les listes
4. Les **blocs de code** nécessitent une ligne vide avant et après

## Outils recommandés

- **Éditeurs :** VS Code, Ghostwriter, Typora
- **Prévisualisation :** Ctrl+Shift+V dans VS Code
- **Convertir MD → PDF :** pandoc
  ```bash
  sudo apt install pandoc
  pandoc fichier.md -o fichier.pdf
  ```
