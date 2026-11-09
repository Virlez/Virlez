# Virlez 👋

**Quality Engineering · QA Automation · Quality Assistance**  
📍 Toulouse / Blagnac · France · [LinkedIn](https://www.linkedin.com/in/andreivaldir/)

Je suis ingénieur QA Automation, spécialisé dans la conception de stratégies de tests, l'architecture E2E et l'accompagnement des équipes de développement. Mon fil conducteur : **rendre les logiciels plus fiables, et rendre leur qualité vérifiable**.

Au quotidien, j'interviens comme **référent et coach QA auprès de plusieurs équipes** : revues obligatoires des modifications de la suite E2E, pair programming avec les développeurs, stratégie de validation des versions et rédaction d'ADR pour les choix de test d'un nouveau produit.

Je m'intéresse aussi à la qualité des produits intégrant de l'IA : tests fonctionnels (OCR, matching de CV, chatbots, reformulation), résistance aux *prompt injections* et workflows d'agents pour assister les activités QA.

## 🔍 Trois projets, trois angles de Quality Engineering

### 🛡️ [Compagnon D&D 5.5 FR](https://github.com/Virlez/compagnon-dd55-fr) — qualité d'un produit distribué

Extension Chrome/Edge pour enrichir et franciser l'expérience D&D 2024 sur Roll20, **publiée et utilisée**.

- **Tests :** Vitest, Playwright, vérification TypeScript et contrôles de sécurité.
- **Mutation testing :** Stryker sur **4 modules ciblés** (sauvegardes, collections, onboarding, URL externes).
- **Résultat documenté :** score de mutation passé de **51,38 % à 97,66 %** après renforcement des tests (mesure du 29 octobre 2026 ; **471 mutations générées**).
- **Garde-fou CI :** seuil de mutation **bloquant à 90 %**, rapports conservés comme artefacts GitHub Actions.
- **Livraison :** checklist de release, contrôles avant publication et documentation des risques résiduels.

📖 [Démarche de mutation testing](https://github.com/Virlez/compagnon-dd55-fr/blob/main/docs/MUTATION-TESTING.md) · [Revue de sécurité](https://github.com/Virlez/compagnon-dd55-fr/blob/main/docs/SECURITY-REVIEW-1.4.2.md) · [Chrome Web Store](https://chromewebstore.google.com/detail/compagnon-dd-55-fr/hamfahkbjnljnmcofgefoimhaabmjalb)

### 🎲 [Rollz](https://github.com/Virlez/rollz) — automatisation et résilience web

Lanceur de dés JDR, accessible en **PWA** et utilisé par des joueurs. Application JavaScript, tests Playwright en TypeScript.

- **Tests E2E multi-navigateurs :** configuration Chromium, Firefox et WebKit.
- **Tests déterministes :** simulation des réponses de RANDOM.ORG pour vérifier des résultats normalement aléatoires.
- **Résilience :** erreurs réseau, réponses HTTP 503, reprise après incident et bascule vers Web Crypto lorsque l'API est indisponible.
- **Parcours utilisateur :** calcul des jets, favoris, historique, traduction, responsive et comportements PWA.
- **Mesure de couverture E2E :** scripts de collecte et de génération de rapports.

🌐 [Essayer Rollz](https://virlez.github.io/rollz/) · [Voir les tests Playwright](https://github.com/Virlez/rollz/tree/main/tests/e2e)

### 🧩 [Rusty VTT](https://github.com/Virlez/rusty-vtt) — stratégie QA sur un développement assisté par IA

Prototype de table virtuelle multijoueur avec un backend Rust (Axum/Tokio). Le développement applicatif a été **largement assisté par des agents IA** ; mon rôle principal a été le **pilotage du projet et de sa stratégie de validation**, et non une expertise de développeur Rust.

- **Pyramide de tests :** tests unitaires Rust, cinq suites d'intégration HTTP et E2E Playwright.
- **Scénarios à risque :** authentification, autorisations, séparation MJ/joueur, persistance et restauration des données.
- **Tests proches du réel :** vrai serveur Rust, échanges HTTP/SSE, plusieurs contextes utilisateurs et données isolées.
- **CI :** exécution de la suite sur les pull requests et conservation des diagnostics en cas d'échec.

📖 [Stratégie et limites de test](https://github.com/Virlez/rusty-vtt/blob/main/docs/TESTING.md)

## 🧰 Outils et pratiques

**Automation & code** : Playwright · TypeScript · C#/.NET · Vitest · Stryker · JavaScript  
**API & données** : REST · Postman · Bruno · SQL Server / T-SQL  
**Industrialisation** : Git · Azure Pipelines · GitHub Actions · CI/CD · tests unitaires, d'intégration et E2E  
**Approche qualité** : stratégie par les risques · Quality Assistance · non-régression · revues de code · ADR · coaching  
**IA & sécurité** : tests fonctionnels IA · prompt injection · outils et agents QA · investigation de vulnérabilités applicatives

## 🤝 Échanger

J'échange volontiers sur l'architecture des tests, le Quality Engineering, les outils QA assistés par IA et l'amélioration des pratiques d'équipe.  
📨 [Me contacter sur LinkedIn](https://www.linkedin.com/in/andreivaldir/)
