MiroCert — Simulation Certifiée d’Opinion Publique

Plateforme propriétaire transformant des simulations brutes en expertises prédictives certifiées et vendables.

Contexte
MiroCert permet à des décideurs (cabinets de conseil, think-tanks, assureurs, avocats) d’obtenir des analyses structurées, traçables et certifiées pour anticiper les réactions collectives.

Architecture & Points forts
- Séparation stricte et non-négociable entre le moteur de simulation (AGPL) et la couche propriétaire
- Certification cryptographique complète des résultats (SHA-256, ECDSA, horodatage RFC 3161)
- Pipeline complet : orchestration → simulation → certification → génération de rapports PDF (30-50 pages)
- API REST performante avec FastAPI

Stack technique
- Python 3.11+ & FastAPI
- Neo4j (graphe de connaissances)
- Docker Compose + architecture conteneurisée
- Certification & traçabilité avancée

Structure du projet
- `src/` : Code propriétaire (API, orchestrator, certification, reporting)
- `infra/docker/` : Moteur de simulation isolé
- `docs/` : Architecture détaillée et décisions techniques

Captures d’architecture à venir dans le dossier `mirocert/assets/`
