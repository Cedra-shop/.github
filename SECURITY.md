# Politique de Sécurité

La sécurité est une priorité absolue pour **Cedra-Shop**, particulièrement compte tenu de notre modèle économique de plateforme E-Commerce manipulant des transactions financières (`Finance`, `Payment` services) et des données d'utilisateurs privées (`Auth`, `Commerce`).

## Versions Supportées

Nous fournissons activement des patchs de sécurité et assurons l'audit des services critiques en production. Les versions suivantes sont maintenues :

| Version | Support Sécurité |
| ------- | ---------------- |
| v2.x.x  | :white_check_mark: Maintenu |
| v1.x.x  | :x: Fin de cycle de vie (EOL) |

## Signaler une Vulnérabilité

**Ne signalez PAS les failles de sécurité ou les fuites via des issues GitHub publiques.**

Si vous découvrez une vulnérabilité de sécurité concernant la Cedra Gateway, le Backend Core, l'IA Engine ou sur un de nos clients (Flutter/NextJS), merci de suivre la procédure de divulgation responsable :

1. Envoyez un email décrivant la vulnérabilité à **security@cedra-shop.com** (ou à l'email de contact direct fourni en privé).
2. Incluez toutes les informations requises pour nous permettre de reproduire et valider l'impact :
   - Microservice ou Repository affecté (ex: `Finance-Service-Rust` ou `Auth-Gateway-Go`).
   - Le protocole concerné (gRPC, HTTP, Kafka topic).
   - Les étapes explicites pour reproduire l'attaque.
   - L'impact direct potentiel.

Nous vous répondrons dans les 48 heures suivant la réception du signalement pour entamer l'investigation et vous communiquer notre roadmap de résolution avant toute publication de correctif ou annonce.
