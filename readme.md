# Karusensei Graphite Dark

Thème sombre pour Visual Studio Code : une interface en **gris purs**, sans aucune
teinte bleutée, autour d'une coloration syntaxique vive.

Deux variantes :

- **Karusensei Graphite Dark**
- **Karusensei Graphite Dark Italic** : commentaires, mots-clés et `this` / `self` en italique.

## Principes

- **Gris neutres uniquement.** Tous les gris de l'interface ont `R = G = B`, ce qui
  donne un graphite mat, sans dominante froide. L'échelle complète est dans
  [grey-palette.md](grey-palette.md).
- **L'éditeur au centre.** Le fond de l'éditeur (`#181818`) est le gris le plus
  sombre de l'espace de travail. L'onglet actif reprend exactement ce fond, et la
  barre d'onglets est plus claire (`#252525`) : l'onglet sélectionné semble se
  prolonger dans l'éditeur.
- **Un seul gris pour le cadre.** La barre d'activité et la barre d'état partagent
  `#323232`, y compris au survol et sur l'élément actif. Seule l'icône change d'état,
  sans carré de fond.
- **Repères discrets.** Les règles verticales et les repères d'indentation
  (`#262626`) se devinent sans attirer l'œil. Le repère du bloc courant ressort un
  peu plus (`#3a3a3a`).
- **Un accent bleu** (`#3691ff`) pour ce qui est actif : liseré de l'onglet,
  élément actif de la barre d'activité, bordure de la barre d'état, badges.

## Interface

| Rôle                              | Hex       |
| --------------------------------- | --------- |
| Fond de l'éditeur, onglet actif   | `#181818` |
| Barre d'onglets, onglets inactifs | `#252525` |
| Onglet survolé                    | `#2e2e2e` |
| Barre d'activité, barre d'état    | `#323232` |
| Règles, repères d'indentation     | `#262626` |
| Texte principal                   | `#b1b1b1` |
| Texte secondaire                  | `#6c6c6c` |
| Bordures                          | `#434343` |
| Accent                            | `#3691ff` |

## Syntaxe

| Portée                     | Hex       |
| -------------------------- | --------- |
| Texte                      | `#b1b1b1` |
| Commentaire                | `#636d83` |
| Mot-clé                    | `#10b1fe` |
| Fonction, méthode          | `#3fc56b` |
| Propriété                  | `#ce9887` |
| Chaîne                     | `#f9c859` |
| Nombre                     | `#ff78f8` |
| Constante                  | `#9f7efe` |
| Balise                     | `#3691ff` |
| Attribut de balise         | `#ff936a` |
| Classe, type, interface    | `#ff6480` |
| Opérateur, ponctuation     | `#7a82da` |

Les commentaires gardent volontairement un gris légèrement bleuté : il les détache
du texte courant.

## Installation

Le thème n'est pas publié sur le Marketplace. Pour l'installer depuis les sources :

```bash
npx @vscode/vsce package
code --install-extension karusensei-graphite-dark-1.0.0.vsix
```

Choisir ensuite **Karusensei Graphite Dark** avec `Preferences: Color Theme`.

Pour le modifier en direct, ouvrir ce dossier dans VS Code et lancer la configuration
**Extension** (`F5`) : la fenêtre de développement recharge le thème à chaque
enregistrement.

## Origine et licence

Karusensei Graphite Dark est dérivé de [Bluloco Dark](https://github.com/uloco/theme-bluloco-dark)
d'uloco, dont il reprend la coloration syntaxique. L'interface a été entièrement
reprise : passage aux gris neutres, fond d'éditeur et hiérarchie des surfaces
redéfinis, onglets, barres et repères retravaillés.

Comme le thème d'origine, il est distribué sous licence
[GNU LGPL v3](LICENSE.txt).
