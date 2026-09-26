# Introduction étape par étape au framework web [Laravel]

**Le cours est en ligne ici : [https://stahe.github.io/laravel-sept-2026/](https://stahe.github.io/laravel-sept-2026/)**

## Auteur

Le cours et l'ensemble de ses codes ont été écrits par **Claude**, l'IA d'Anthropic, **unique auteur**, à la demande de Serge Tahé (septembre 2026).

## Présentation

Ce cours enseigne pas à pas la construction d'une application web MVC avec le framework **Laravel 13** et le langage **PHP 8.4**. Les pages HTML y sont fabriquées par le serveur, avec des vues **Blade**, sans framework JavaScript côté navigateur.

Il transpose dans le monde PHP le cours [Introduction étape par étape au framework web [Flask]](https://stahe.github.io/flask-sept-2026/), lui-même issu des cours [Spring MVC](https://stahe.github.io/springmvc-sept-2026/), [ASP.NET Core MVC](https://stahe.github.io/aspnetcoremvc-sept-2026/) et [NestJS](https://stahe.github.io/nestjs-html-sept-2026/). Les exemples portent les mêmes numéros et traitent les mêmes sujets : on peut comparer les frameworks exemple par exemple.

## Contenu

| Chapitre | Sujets | Exemples |
|---|---|---|
| Actions, routage, réponses | routes, contrôleurs, réponses, redirections, conteneur de services | 01 à 06 |
| Le modèle d'une action | paramètres de la requête, liaison, validation, requêtes POST | 07 à 12 |
| La vue et son modèle | Blade, gabarit, composants, formulaires, validation, Post/Redirect/Get, protection anti-CSRF | 13 à 21 |
| Internationalisation | une application en français et en anglais | 22 |
| Portées des données | requête, session, cache, cookies | 23 |
| Le cycle de vie d'une requête | middlewares, liaison des paramètres, gestionnaires d'exceptions | 24 |
| Authentification et autorisation | JWT dans un cookie, gardes, rôles, captcha, limitation des tentatives | 25 à 27 |
| Architecture en couches | web / métier / DAO avec Eloquent et MySQL | 28 |
| Étude de cas | **RdvMedecins**, une application de prise de rendez-vous médicaux, commentée fichier par fichier | - |

L'étude de cas `rdvmedecins2-laravel` gère trois rôles (administrateur, médecins, patients) : agendas, réservations, gestion des médecins et des clients, création de compte protégée par captcha, interface FR / EN. Elle utilise la même base de données `dbrdvmedecins2` que les autres versions de l'application.

## Prérequis

- PHP 8.4 ou plus récent (extensions `intl`, `mbstring`, `openssl`, `pdo_mysql`) ;
- Composer 2 ;
- MySQL 8 ou MariaDB (Laragon sous Windows) ;
- Visual Studio Code avec les extensions PHP Intelephense et Laravel ;
- curl.

Les codes sont téléchargeables depuis le site du cours. Les dossiers `vendor` n'y figurent pas : `composer install` les fabrique, une fois dans le dossier `exemples`, une fois dans le dossier `rdvmedecins2-laravel`.
