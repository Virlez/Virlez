**Quality Engineering · QA Automation · Quality Assistance**  

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

### 🎲 [Rollz](https://github.com/Virlez/rollz) — automatisation, mutation testing et résilience web

Lanceur de dés JDR accessible en **PWA**, utilisé par des joueurs. Application JavaScript avec un moteur partagé TypeScript et des tests Playwright/Vitest.

- **Pyramide de tests rééquilibrée :** **157 tests unitaires** et **122 scénarios E2E par navigateur** documentés ; les variantes de calcul ont été déplacées au niveau unitaire lorsque le navigateur n'apportait pas de valeur supplémentaire.
- **Mutation testing :** Stryker sur **8 fichiers métier** (parseurs, moteurs, aléatoire, limites et orchestration) ; score documenté passé de **17,41 % à 93,96 %** sur **1 522 mutations**. Le score inclut 7 timeouts et ne représente pas toute l'application.
- **CI :** seuil de mutation **bloquant à 90 %** ; tests unitaires et E2E Chromium sur les PR, puis Chromium/Firefox/WebKit sur `main`, avec rapports et traces.
- **Déterminisme et résilience :** tirages contrôlés, simulation des réponses de RANDOM.ORG, erreurs HTTP/réseau, reprise et bascule vers Web Crypto.
- **Parcours utilisateur :** formules, favoris, historique, responsive, localisation et PWA ; scripts de mesure de couverture E2E.

*En cours : extension de la couche de tests d'intégration.*

🌐 [Essayer Rollz](https://virlez.github.io/rollz/) · [Stratégie et résultats de mutation](https://github.com/Virlez/rollz/blob/main/docs/MUTATION_TESTING.md) · [Tests E2E](https://github.com/Virlez/rollz/tree/main/tests/e2e)

### 🧩 [Rusty VTT](https://github.com/Virlez/rusty-vtt) — stratégie QA sur un développement assisté par IA

Prototype de table virtuelle multijoueur avec backend Rust (Axum/Tokio). Le développement est **largement assisté par des agents IA** ; mon rôle est d'abord le **pilotage du projet et de sa stratégie de validation**, sans revendiquer une expertise de développement Rust.

- **Tests multicouches :** tests unitaires Rust, **9 propriétés génératives** avec `proptest`, **7 suites d'intégration HTTP** sur le véritable serveur et **11 parcours Playwright sur 3 moteurs** (33 exécutions E2E).
- **Confidentialité et sécurité :** projections MJ/joueur, contrôle des autorisations, données privées, notifications HTTP/SSE et absence de fuite entre utilisateurs.
- **Persistance et concurrence :** sauvegardes corrompues, échecs réels d'écriture/renommage, reprise après incident, redémarrages et mutations simultanées sans perte de données.
- **Résilience réseau :** reconnexion SSE après interruption réelle, rattrapage des événements, conservation de session et protection des messages privés.
- **Mutation testing Rust :** `cargo-mutants` ciblé sur les règles critiques (authentification, permissions, visibilité, quotas) ; campagne **à déclenchement manuel**, sans score global annoncé.
- **CI :** tests Rust, HTTP et E2E Chromium/Firefox/WebKit sur les pull requests, avec diagnostics d'échec.

*En cours : enrichissement des scénarios de test.*

📖 [Périmètre, stratégie et limites](https://github.com/Virlez/rusty-vtt/blob/main/docs/TESTING.md) · [Configuration des mutations](https://github.com/Virlez/rusty-vtt/blob/main/.cargo/mutants.toml)

## 🧰 Outils et pratiques

**Automation & code** : Playwright · TypeScript · C#/.NET · Vitest · Stryker · JavaScript  
**API & données** : REST · Postman · Bruno · SQL Server / T-SQL  
**Industrialisation** : Git · Azure Pipelines · GitHub Actions · CI/CD · tests unitaires, d'intégration et E2E  
**Approche qualité** : stratégie par les risques · Quality Assistance · mutation testing · property-based testing · non-régression · revues de code · ADR · coaching  
**IA & sécurité** : tests fonctionnels IA · prompt injection · outils et agents QA · investigation de vulnérabilités applicatives

