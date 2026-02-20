# Guide de Contribution - Cedra-Shop

Bienvenue dans l'équipe d'ingénierie de **Cedra-Shop** ! Ce document décrit les procédures et bonnes pratiques pour intervenir sur notre architecture microservices distribuée en interne.

## 🚀 Notre Stack Technique

Avant de pousser du code, assurez-vous de bien maîtriser ou comprendre les bases des technos utilisées dans le(s) service(s) visé(s) :
- **Core / Backend** : Go, Rust, Java
- **Frontend / Mobile** : TypeScript, Next.js, Flutter, Dart
- **Data / IA** : Python, PyTorch, TensorFlow
- **Infrastructure / Data Layer** : Docker, Nomad, Valkey, Kafka

## 🛠 Environnement de Développement

1. **Cloner le répertoire**
   ```bash
   git clone https://github.com/Cedra-shop/<nom-du-repo>.git
   cd <nom-du-repo>
   ```

2. **Démarrer l'infrastructure locale**
   Consultez le `README.md` spécifique à chaque microservice. Beaucoup de services dépendent de la Gateway (Traefik), Valkey, Postgres ou Kafka. Des commandes Makefile (ex. `make dev`) sont souvent fournies.
   
3. **Tests de résilience**
   Assurez-vous de lancer et passer tous les tests unitaires avant de l'envoyer en PR. Notre domaine e-commerce (Finance, Order, Payment) nécessite une sécurité et une précision de 100%.

## 🤝 Flux de travail (Workflow)

1. Ciblez une issue existante ou créez-en une nouvelle (voir nos Issues Templates).
2. Créez une branche à partir de `main` : `git checkout -b feature/nom-de-la-feature` (ou `fix/...`).
3. Commitez vos changements avec des messages clairs (voir *Conventions de Commit*).
4. Poussez votre branche sur le dépôt distant.
5. Ouvrez une **Pull Request** vers la branche `main` et remplissez le template PR.
6. Demandez une revue à l'équipe Engineering.

## 📝 Conventions de Commit

Nous utilisons la convention [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/). Exemples :
- `feat(order): implémentation du système d'event sourcing Rust`
- `fix(auth): résolution de la fuite mémoire dans le middleware JWT`
- `docs(profile): mise à jour du diagramme d'architecture Mermaid`
- `perf(cache): optimisation des accès distribués Valkey`

## 💬 Code de Conduite

Veuillez lire et respecter notre [Code de Conduite](CODE_OF_CONDUCT.md) lors des échanges dans nos Repositories ou réunions.

---
*L'équipe d'ingénierie Cedra-Shop.*
