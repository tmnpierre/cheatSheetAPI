# Fiche de référence : Concepts des API

## Concepts de base

### 1. API (Interface de Programmation d'Application)
- **Description** : Comme un menu dans un restaurant qui vous indique ce que vous pouvez commander à partir d'un programme informatique.

### 2. Architecture Client-Serveur
- **Description** : Le client (vous) demande des données ou un service, et le serveur (un système distant) répond, comme une interaction dans un restaurant.

### 3. Consommation d'API
- **Description** : Utilisation de l'API pour demander des informations spécifiques ou des services, similaire à la commande de plats à partir d'un menu de restaurant.

## Interaction avec les serveurs

### 4. Verbes HTTP
- **GET** : Demande d'informations, comme consulter le menu.
- **POST** : Envoi d'informations pour créer quelque chose de nouveau, comme commander un plat qui n'est pas répertorié.
- **PUT** : Mise à jour des informations existantes, comme modifier une commande entière.
- **PATCH** : Mise à jour partielle, comme modifier une partie d'une commande.
- **DELETE** : Suppression de quelque chose, comme annuler une commande.

### 5. Comprendre ce qu'est une route dans une API

- **Ville (API)** : La ville représente l'ensemble de l'API, un système complexe avec diverses fonctions et services.
- **Adresse (Route)** : Une route dans une API est comme une adresse spécifique dans cette ville. Tout comme chaque adresse mène à un bâtiment ou un lieu spécifique, chaque route dans une API conduit à une fonction ou une ressource spécifique.
- **Signalisation (Documentation de l'API)** : Tout comme les panneaux dans une ville vous aident à trouver une adresse, la documentation de l'API guide les développeurs pour accéder aux bonnes routes et comprendre ce qu'elles font.
- **Modes de transport (Requêtes HTTP)** : Les différents modes de transport (voiture, vélo, à pied) peuvent être vus comme les différents types de requêtes HTTP (GET, POST, etc.). En fonction du type de requête, votre "voyage" vers l'adresse (route) sera différent.
- **Destination (Ressource ou Service)** : Une fois arrivé à l'adresse (route), vous accédez à la destination souhaitée, qui peut être une information spécifique, un service ou une interaction avec le système, tout comme arriver dans un restaurant, une bibliothèque ou un parc dans une ville.

## Autres concepts

6. **Charge utile (Payload) dans les requêtes HTTP** :
   - La charge utile dans une requête HTTP fait référence aux données qui sont envoyées avec la requête elle-même. Imaginez cela comme le contenu d'une lettre que vous envoyez par la poste. Lorsque vous interagissez avec un serveur via une requête HTTP, que ce soit pour récupérer des informations, soumettre des données, ou effectuer une action, vous incluez généralement des données spécifiques en tant que charge utile.
   - Cette charge utile peut prendre différentes formes, notamment du texte brut, des données structurées au format JSON ou XML, des fichiers binaires tels que des images ou des vidéos, etc. Elle contient les informations que le serveur doit traiter pour répondre à votre demande de manière appropriée. Par exemple, lors de l'envoi d'un formulaire en ligne, les informations que vous entrez dans les champs du formulaire constituent la charge utile de la requête HTTP.

7. **Modèle MVC (Modèle-Vue-Contrôleur)** :
   - Le modèle, la vue et le contrôleur sont des composants clés de l'architecture de conception MVC (Modèle-Vue-Contrôleur), largement utilisée dans le développement logiciel. Cette architecture permet de mieux organiser le code d'une application en le séparant en trois parties distinctes :
     - **Modèle** : Le modèle gère et traite les données de l'application. Il est responsable de la logique métier, de l'accès aux données et de leur manipulation. Vous pouvez le considérer comme la cuisine d'un restaurant, où la préparation des plats a lieu.
     - **Vue** : La vue est responsable de la présentation des données à l'utilisateur final. Elle affiche les informations de manière conviviale et interagit avec l'utilisateur. Vous pouvez la comparer à la salle à manger d'un restaurant, où les plats sont servis à la table du client.
     - **Contrôleur** : Le contrôleur agit comme un intermédiaire entre le modèle et la vue. Il gère les interactions entre les deux, en traitant les demandes de l'utilisateur et en mettant à jour le modèle en conséquence. Le contrôleur est similaire au serveur dans un restaurant, qui prend les commandes des clients, les transmet à la cuisine, puis sert les plats une fois qu'ils sont prêts.
   - Cette division claire des responsabilités dans l'architecture MVC facilite la maintenance, la réutilisation du code et l'extensibilité des applications logicielles.

8. **Architecture REST (Representational State Transfer)** :
   - L'architecture REST est un ensemble de principes et de conventions largement adoptés pour concevoir des services Web et des API. Elle est souvent comparée à l'étiquette et aux règles de comportement dans un restaurant, car elle définit comment les demandes et les réponses entre clients et serveurs doivent être structurées et gérées.
   - REST repose sur plusieurs principes clés, notamment l'utilisation d'URLs pour identifier les ressources, l'utilisation de méthodes HTTP standard (GET, POST, PUT, DELETE, etc.) pour effectuer des actions sur ces ressources, et la représentation des ressources sous forme de données (par exemple, JSON ou XML).
   - En suivant les principes de REST, les services Web deviennent plus simples à comprendre, à utiliser et à intégrer avec d'autres systèmes, ce qui les rend très populaires dans le développement d'applications modernes, en particulier les applications Web et mobiles.

### 9. Étatful vs Stateless (Avec état vs Sans état)
- **Étatful** : Le serveur se souvient des interactions précédentes.
- **Sans état** : Chaque demande est traitée indépendamment, sans mémoire des interactions passées.

### 10. URL / URI / URN (Adresse Web / Identifiant de Ressource Uniforme / Nom de Ressource Uniforme)

- **URL (Uniform Resource Locator)** : Une URL est une forme spécifique d'URI. Elle est principalement utilisée pour localiser et accéder à une ressource sur Internet. Une URL comprend généralement plusieurs composants, tels que le protocole (par exemple, HTTP ou HTTPS), le nom de domaine (par exemple, www.example.com), le chemin vers la ressource sur le serveur (par exemple, /page1), et éventuellement des paramètres (par exemple, ?id=123) ou des ancres (#section1). Les URL sont couramment utilisées pour accéder à des sites Web, des images, des vidéos et d'autres ressources en ligne de manière précise.

- **URI (Uniform Resource Identifier)** : Une URI est un terme plus général qui englobe à la fois les URL et les URN. Une URI peut être utilisée pour identifier de manière unique n'importe quelle ressource, qu'elle soit située sur Internet ou non. Les URIs sont utilisées dans divers contextes, notamment les liens hypertextes, les identifiants de fichiers sur un système de fichiers local, les identifiants de bases de données, etc. Les URIs servent principalement à désigner et à identifier les ressources de manière unique.

- **URN (Uniform Resource Name)** : Une URN est un sous-ensemble des URIs spécifiquement utilisé pour attribuer un nom unique à une ressource sans spécifier son emplacement ou sa méthode d'accès. Les URNs sont conçues pour être persistantes et indépendantes de l'emplacement, ce qui signifie qu'elles doivent rester valides même si la ressource change d'emplacement ou de méthode d'accès. Les URNs sont moins courantes que les URLs, mais elles sont utilisées dans des contextes tels que la dénomination de fichiers, la résolution de noms et l'attribution de noms uniques à des ressources numériques.

En résumé, une URL est un type spécifique d'URI qui inclut des informations détaillées sur l'emplacement d'une ressource sur Internet, une URN est un autre type d'URI qui attribue un nom unique à une ressource sans spécifier son emplacement, et une URI est un terme plus large qui englobe les deux. Toutes les URLs sont des URIs, toutes les URNs sont des URIs, mais toutes les URIs ne sont pas nécessairement des URLs ou des URNs.

### 11. Chemin relatif vs Chemin absolu
- **Chemin absolu** : Une référence complète à partir de la racine du système de fichiers.
- **Chemin relatif** : Une référence basée sur l'emplacement actuel.

### 12. ORM (Mapping Objet-Relationnel) vs ODM (Mapping Objet-Document)
- **ORM** : Traduit entre les données stockées dans les tables et leur utilisation dans les objets.
- **ODM** : Traduit pour les bases de données basées sur des documents (comme le JSON).

### 13. Middleware (Intergiciel)
- **Description** : Agit comme un intermédiaire dans un processus, ajoutant ou modifiant des éléments dans un système informatique.

## Codes d'état HTTP

| Catégorie | Description |
|----------|-------------|
| 2xx      | Succès : La demande a été reçue, comprise et acceptée. |
| 3xx      | Redirection : Des actions supplémentaires doivent être entreprises pour finaliser la demande. |
| 4xx      | Erreurs côté client : La demande contient des erreurs ou ne peut pas être traitée. |
| 5xx      | Erreurs côté serveur : Le serveur n'a pas réussi à traiter une demande valide. |

### Codes d'état spécifiques
- **418 Je suis une théière** : Une blague du 1er avril, indiquant que la machine est une théière, pas une cafetière.
- **420 Améliorez votre calme** : Utilisé par Twitter pour indiquer que le client a été limité en termes de taux pour avoir effectué trop de demandes.