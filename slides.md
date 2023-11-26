---
titleTemplate: '%s'
colorSchema: light
theme: seriph
background: https://source.unsplash.com/1920x1080/?developer-computer
highlighter: shiki
lineNumbers: true
info: false
css: unocss
hideInToc: true 
---

# Comment participer à l'open source ?

Guide pratique et retour d'expérience

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
layout: center
hideInToc: true
---

# De quoi on parle ?

<Toc />

---
layout: center
class: text-center
src: ./pages/presentations.md
---

---
layout: section
title: Introduction & définition
level: 1
---

# L'Open source

> N'importe qui peut voir, modifier et distribuer le code à sa convenance.

<!-- On y reviendra à la fin. Question ouverte: "qui fait de l'open source ici?" -->

---
title: Qu'est-ce qu'une participation ?
level: 2
layout: center
---

# Qu'est-ce qu'une participation ?

<v-clicks depth="2">

- Code
    - Feature
    - Fix
- Documentation
- Bug report, discussions ..

</v-clicks>

<!-- Question ouverte sur ce que les gens considèrent une participation -->

---
title: Motivation
level: 2
layout: center
---

# Motivations

<v-clicks>

- Sensation d'aider/appartenir à plus qu'une entreprise
- Sensation d'oeuvrer pour la communauté
- Apprendre sur une technologie, se former
- Être acteur des outils qu'on utilise

</v-clicks>

<!-- Question ouverte encore sur les motivations des gens dans la salle -->

---
title: Obstacles
level: 2
layout: center
---

# Obstacles

- Manque de temps
- Complexité du sujet
- Peur du jugement
- Difficulté à commencer
- ...

<!-- Obstacles : Manque de temps, Complexité du sujet, Difficulté à commencer, Peur du jugement -->

---
title: Mes PR dans le temps
level: 1
---

# Mes PR en étude

| Année                        | Projet                                                                                                  | Commentaires                        |
|------------------------------|---------------------------------------------------------------------------------------------------------|-------------------------------------|
| Première année               | [JetBrains/swot](https://github.com/JetBrains/swot)                                                     |                                     |
| Deuxième année               | [rectorphp/rector](https://github.com/rectorphp/rector)                                                 | Lien incorrect, doc!                |
|                              | [FriendsOfSylius/SyliusImportExportPlugin](https://github.com/FriendsOfSylius/SyliusImportExportPlugin) | Ligne en doublon                    |
|                              | [EasyCorp/EasyAdminBundle](https://github.com/EasyCorp/EasyAdminBundle)                                 | Compatibilité vers PHP 7.4          |
|                              | [api-platform/*](https://github.com/api-platform/*)                                                     | Mise à jour de l'année en footer    |
| Troisième année              | [symfony/symfony-docs](https://github.com/symfony/symfony-docs)                                         | Ajout du @Ignore à la documentation |
| Quatrième & cinquième années | [symfony/symfony](https://github.com/symfony/symfony)                                                   | Ajout du AMQPS avec documentation   |

---
layout: two-cols
hideInToc: true
---

# Première PR

<img src="/first-pr.png">

::right::
# Critique

- Pas de description, version cible...
- Des remerciements
- Un merge rapide

---
layout: two-cols
hideInToc: true
---

# Un peu de maturité

<img src="/pr-amqps.png">

::right::

<img src="/pr-amqps2.png">

<img src="/pr-ratelimiter.png">

<!-- Beaucoup de retour, de discussion, de support et le suivi des guides -->

---
hideInToc: true
---

# 7 ans d'existence !

```markdown
Contributing
------------

[...]

* [Reviewing issues/pull requests][0]
* [Reporting a Bug][1]
* [Submitting a Patch][2]
* [Symfony Core Team][3]
* [Security Issues][4]
* [Running Symfony Tests][5]
* [Our Backwards Compatibility Promise][6]
* [Coding Standards][7]
* [Conventions][8]

[0]: https://symfony.com/doc/current/contributing/community/reviews.html
[1]: https://symfony.com/doc/current/contributing/code/bugs.html
[2]: https://symfony.com/doc/current/contributing/code/patches.html
[3]: https://symfony.com/doc/current/contributing/code/core_team.html
[4]: https://symfony.com/doc/current/contributing/code/security.html
[5]: https://symfony.com/doc/current/contributing/code/tests.html
[6]: https://symfony.com/doc/current/contributing/code/bc.html
[7]: https://symfony.com/doc/current/contributing/code/standards.html
[8]: https://symfony.com/doc/current/contributing/code/conventions.html
```

---
hideInToc: true
---

# La PR la plus complexe jusque la

<img src="/pr-flasky.png"/>

```diff
-    - echo serialize_precision=14 >> php.ini-min
+    - echo serialize_precision=-1 >> php.ini-min
```

---
hideInToc: true
---

# Des PR pour s'améliorer

Upgrade : SF, PHP 8.0, Docker, Github action..

- FriendsOfSylius/SyliusImportExportPlugin
- FriendsOfSymfony/oauth2-php
- FriendsOfSymfony/FOSOAuthServerBundle
- Sylius/Sylius-Standard
- Speicher210/CloudinaryBundle
- brefphp/extra-php-extensions
- sspooky13/yaml-standards

<!-- C'est une partie de mon taf aujourd'hui ! Annecdote client -->

---
layout: center
title: bonus
level: 2
---

# Pour s'amuser

https://github.com/RageCage64/is-even/pull/24

```php
<?php declare(strict_types=1);
function isEven(int $x) {
    return !($x & 1);
}
?>
```

---
title: Statistiques
level: 2
---

# Total de PR

| Repo                                     | Nb | Accepté |
|------------------------------------------|----|---------|
| FriendsOfSylius/SyliusImportExportPlugin | 10 | 8       |
| Sylius/*                                 | 10 | 2       |
| symfony/*                                | 9  | 5       |
| api-platform/*                           | 6  | 6       |
| EasyCorp/EasyAdminBundle                 | 3  | 3       |
| ...                                      | 18 | 6       |

53% de PR mergés !

---
layout: section
title: Conclusions
level: 1
---

# Conclusions

---
layout: center
title: Logiciel libre
level: 2
---

# Différencier open source et logiciel libre

## Rappel

Définition de l'open source:
> N'importe qui peut voir, modifier et distribuer le code à sa convenance.

### Citation GNU.org

> Ce point de vue ne prend en compte que les avantages pratiques des logiciels libres et évite soigneusement les questions plus fondamentales de liberté et de solidarité sociale que soulève le mouvement du logiciel libre. <br/>
> Si vous pensez que la liberté et la communauté sont importantes en soi, rejoignez-nous en utilisant fièrement le terme « logiciel libre » et aidez à faire passer le message.

<!-- Il existe une distinction entre ces deux notions, le (mvnt log libre) est imprégné d'une philosophie politique, mettant l'accent sur la liberté de l'utilisateur, le contrôle du logiciel utilisé et la lutte contre les restrictions imposés par les logiciels propriétaires -->

---
layout: center
title: Problématique financière
---

# Problématique financière

En janvier 2022, un contributeur corrompt des fichiers de bibliothèques open source sur GitHub et le registre de logiciels npm - faker.js et colors.js en introduisant une boucle infinie dans son code source afin de protester contre l'utilisation gratuite de son travail par de grosses entreprises informatique sans contrepartie financière pour son travail bénévole.

<img src="/opencollective-apip.png" />

Sylius = 600 installation par jour ^2.6

---
hideInToc: true
---

<img src="/opencollective-apip.png" />

---
layout: end
hideInToc: true
---

<img src="/Meetup 28_11_2023 QRCode.png" alt="QRcode vers vote openfeedback" height="250px" width="250px" />

<!-- Remercier le staff AFUP et encourager à s'inscrire & voter pour les sujets de l'AFUP -->