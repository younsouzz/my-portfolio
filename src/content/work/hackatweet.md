---
title: Hackatweet
publishDate: 2023-01-01 00:00:00
img: /assets/stock-3.jpg
img_alt: Page d'accueil du site internet hackatweet
description: |

tags:
  - React
  - Twitter
  - SPA
---

<a href="https://hackatweet-frontend-two.vercel.app">Lien vers le site</a>

#### Intro

Création d'une SPA (Single Page Application) basée sur Twitter.

Réalisation de toute la partie frontend et backend.

Implémentation de TDD pour certaines fonctionnalités (par exemple la vérification des champs saisis).

#### Login

La page login vous permet de vous créer un compte ou de vous connecter à l’application.

Au clic sur les boutons "Sign up" ou "Sign in", une modale s’ouvre avec les champs de saisie correspondants à l’action effectuée.

Dans le cas d'un Sign in, au clic sur le bouton dans la modale, l’application communique avec le backend et si les informations sont correctes, l’utilisateur est redirigé vers la page d'accueil.

Dans le cas d’un Sign up, les informations de l’utilisateur sont enregistrées en BDD.

Utilisation d'un token et hashage du mot de passe.

#### Page d'accueil

La page d’accueil est découpée en trois sections.

La première à gauche affiche un logo qui fait aussi office de bouton pour revenir à cette page, les informations de l’utilisateur et un bouton logout.

La partie du milieu sert à ajouter un tweet et à voir le fil des tweets effectués par tous les utilisateurs.

Enfin, la partie de droite affiche les "Trends", c'est-à-dire tous les hashtags qui ont été utilisés et le nombre de fois qu’ils l’ont été.

#### Tweets

Blocage de l'écriture d'un tweet à 280 caractères.

Si un tweet appartient à l’utilisateur connecté, il peut le liker mais aussi le supprimer mais si ce n’est pas le sien, il aura seulement la possibilité de le liker.

Enfin, la page hashtag s’affiche lorsque l’utilisateur clique sur un des hashtags dans la section Trends. Cette action redirige vers une URL personnalisée reprenant le nom de la page et le nom du hashtag (par exemple: /hashtag/hello pour #hello).

La barre de recherche permet de chercher d’autres hashtags, à chaque recherche l’url doit se mettre à jour. Si aucun tweet ne comporte le hashtag recherché, le message "No tweets found with #hashtagname" s’affiche.

Au clic sur le logo, l’utilisateur revient sur la page d’accueil.