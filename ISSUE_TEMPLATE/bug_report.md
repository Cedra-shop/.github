---
name: "🐛 Signaler un Bug"
about: Créer un rapport détaillé pour nous aider à améliorer l'infrastructure et les applications Cedra-Shop.
title: "[BUG] "
labels: bug
assignees: ''
---

## 📝 Description du Bug
<!-- Une description claire et concise de l'erreur ou du bug constaté. -->

## 🔁 Étapes de reproduction
Étapes pour reproduire le comportement :
1. Via tel service, envoyer une requête gRPC / HTTP vers '...'
2. Déclencher un événement dans le topic Kafka '...'
3. Vérifier la réaction dans '...' (Cache, DB)
4. Voir le plantage

## ✅ Comportement attendu
<!-- Une description de ce que vous vous attendiez à voir se produire. -->

## 💻 Environnement technique
- **Microservice affecté** : [ex: Order (Rust), Commerce (Go), AI Engine (Python), Web (NextJS)]
- **Environnement de déploiement** : [ex: Local, On-Premise (Nomad), CI]
- **Versions** : [ex: Go 1.21, Rust 1.70, Flutter 3.10]
- **OS client** (seulement si bug frontend) : [ex: macOS, iOS 16, Android 13]

## 📋 Contexte supplémentaire et Logs
<!-- Ajoutez ici tout contexte, erreur de log (Audit Service), traces (Jaeger/Telemetry) ou capture d'écran de l'incident. -->
