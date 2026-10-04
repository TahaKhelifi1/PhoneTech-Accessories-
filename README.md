# PhoneTech Accessories

## 1. Présentation du projet

PhoneTech Accessories est un site web développé avec WordPress pour une boutique spécialisée dans les accessoires pour smartphones.

Le site permet de présenter les produits, publier des articles et fournir aux visiteurs les informations nécessaires pour contacter l'entreprise.

## 2. Technologies et outils utilisés

* WordPress
* PHP
* MySQL
* HTML / CSS / JavaScript
* XAMPP
* Elementor
* WooCommerce
* Contact Form 7
* Yoast SEO
* Thème Hello Elementor

## 3. Étapes de réalisation

### 3.1 Installation de l'environnement

* Installation de XAMPP.
* Démarrage des services Apache et MySQL.
* Création de la base de données.
* Installation de WordPress dans le dossier `htdocs/phonetech`.

### 3.2 Configuration de WordPress

* Configuration du nom du site : PhoneTech Accessories.
* Configuration des permaliens.
* Installation et activation des extensions nécessaires.
* Installation et utilisation du thème Hello Elementor.

### 3.3 Création des pages

Les principales pages du site sont :

* **Home** : présentation de l'entreprise et mise en avant des produits.
* **Shop** : catalogue des accessoires disponibles.
* **About Us** : présentation de l'entreprise.
* **Blog** : publication des articles.
* **Contact** : informations de contact.

Les pages **Cart**, **Checkout** et **My Account** sont fournies et gérées par WooCommerce.

### 3.4 Création du catalogue

WooCommerce a été utilisé pour créer et gérer les produits.

Le catalogue contient au moins 10 accessoires, notamment :

* Coques de protection
* Chargeurs rapides
* Câbles USB-C
* Écouteurs sans fil
* Casques Bluetooth
* Power Banks
* Supports pour téléphone
* Supports pour voiture

### 3.5 Création du Blog

Trois articles ont été publiés :

1. **Mobile Accessories Trends**
2. **Smartphone Maintenance Tips**
3. **New Technology Trends**

### 3.6 Personnalisation et tests

* Personnalisation des pages du site.
* Vérification de l'affichage des produits.
* Vérification des articles.
* Vérification de la navigation.
* Test du fonctionnement général du site.

## 4. Architecture de WordPress

Le site utilise une architecture principalement monolithique.

### Couche présentation

Elle correspond à l'interface visible par les utilisateurs. Elle est composée du thème WordPress, des pages, des templates, du HTML, du CSS et du JavaScript.

### Couche applicative

Elle est principalement basée sur PHP. WordPress gère la logique de l'application, les pages, les articles, les utilisateurs, les extensions et les fonctionnalités du site.

### Couche données

Les données sont stockées dans une base de données MySQL. Elle contient notamment les utilisateurs, pages, articles, produits, réglages et données des extensions.

### Fonctionnement

Le navigateur envoie une requête au serveur web. WordPress traite cette requête, exécute le code PHP nécessaire et récupère les données depuis la base de données. Le résultat est ensuite envoyé au navigateur sous forme de page web.

## 5. Architecture monolithique vs microservices

| Critère       | Architecture monolithique                            | Architecture microservices                       |
| ------------- | ---------------------------------------------------- | ------------------------------------------------ |
| Organisation  | Une seule application regroupant les fonctionnalités | Plusieurs services indépendants                  |
| Déploiement   | Déploiement de l'ensemble de l'application           | Déploiement indépendant de chaque service        |
| Complexité    | Plus simple                                          | Plus complexe                                    |
| Maintenance   | Centralisée                                          | Chaque service peut être maintenu séparément     |
| Évolutivité   | Mise à l'échelle de l'application                    | Mise à l'échelle service par service             |
| Communication | Communication interne                                | Communication via API ou messages                |
| Adaptation    | Adaptée aux petits et moyens projets                 | Adaptée aux applications complexes et évolutives |

### Architecture monolithique

L'architecture monolithique regroupe les différentes fonctionnalités dans une même application.

**Avantages :**

* Installation simple.
* Développement rapide.
* Maintenance relativement facile pour un petit projet.
* Déploiement simple.

**Inconvénients :**

* L'évolution peut devenir plus difficile lorsque l'application devient importante.
* Une modification peut avoir un impact sur plusieurs parties du système.
* La mise à l'échelle est généralement globale.

### Architecture microservices

L'architecture microservices divise une application en plusieurs services indépendants. Chaque service possède une responsabilité spécifique et peut communiquer avec les autres services via des API.

**Avantages :**

* Services indépendants.
* Déploiement séparé.
* Mise à l'échelle service par service.
* Adaptée aux grandes applications.

**Inconvénients :**

* Architecture plus complexe.
* Communication entre les services à gérer.
* Déploiement et supervision plus difficiles.

## 6. Architecture utilisée dans PhoneTech Accessories

PhoneTech Accessories utilise une architecture principalement monolithique avec WordPress.

Le cœur de WordPress, le thème et les extensions sont intégrés dans la même application. WooCommerce ajoute les fonctionnalités liées à la gestion du catalogue et des produits.

Cette architecture est adaptée au projet car elle permet de développer et gérer facilement un site vitrine et e-commerce de petite ou moyenne taille.

## 7. Sauvegarde du projet

Le projet est sauvegardé avec deux éléments principaux :

### Base de données

La base de données a été exportée depuis phpMyAdmin au format SQL.

### Fichiers

Le dossier complet du site WordPress `phonetech` a été copié depuis :

`C:\xampp\htdocs\phonetech`

Ces deux éléments permettent de conserver une sauvegarde complète du projet.

## 8. Structure de livraison

```text
PhoneTech_Accessories/
│
├── README.md
│
├── Database/
│   └── phonetech_db.sql
│
└── Website/
    └── phonetech/
```

## 9. Conclusion

Ce projet a permis de mettre en pratique la création et la gestion d'un site web avec WordPress, l'utilisation de WooCommerce pour la gestion des produits et l'utilisation d'extensions pour améliorer les fonctionnalités du site.

Il a également permis de comprendre les principales différences entre une architecture monolithique et une architecture microservices.
