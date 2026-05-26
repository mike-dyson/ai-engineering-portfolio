Rap Oracle — Architecture Backend & Moteur Économique Complexe

Plateforme de jeu mobile avec économie dynamique, marketplace P2P et systèmes temps réel.

Contexte
Rap Oracle est une application mobile de simulation et trading de cartes d’artistes rap français, avec un moteur économique sophistiqué et des mécaniques compétitives (Clash PvP).

Défis techniques majeurs
- Conception d’un moteur économique avancé (pricing dynamique, rareté, dilution logarithmique)
- Architecture Double-Bassin (Market + Scouting Pool) avec promotions automatiques
- Système anti-abus complet (rate limiting, cooldowns, optimistic locking)
- Gestion asynchrone avec files d’attente pour les jobs différés
- Clash PvP en temps différé avec snapshots et résolution basée sur données externes
- Synchronisation temps réel (WebSocket + Push Notifications)

Architecture & Points forts
- Economy Engine V2 : Pricing intelligent, stock limité, multiplicateurs de risque
- BullMQ + Redis : Orchestration avancée des jobs asynchrones
- The Drop : Cron hebdomadaire avec harvesting et rééquilibrage
- Architecture prête pour scaler (Provider-Agnostic)

Stack technique
- Backend : Node.js + TypeScript, Express, Socket.IO
- Base de données : PostgreSQL
- Queues : BullMQ + Redis (Upstash)
- Storage*: Supabase (CDN)
- Mobile : React Native + Expo, Zustand
- Temps réel : WebSocket + Push Notifications

Captures d’architecture à venir dans le dossier `rap-oracle/assets/`
