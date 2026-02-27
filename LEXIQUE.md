# Lexique technique - Cybersécurité, IA, Infra et Dev

Version Markdown lisible du lexique public.

Source de vérité: les fichiers JSON dans `data/`.

## Cybersécurité

### ANSSI
- ID: `anssi`
- Catégorie: `cyber`
- Définition courte: Autorité nationale française en cybersécurité et sécurité numérique.
- Définition: L'ANSSI publie des recommandations, guides et positions officielles pour renforcer la sécurité des organisations en France. Ses documents servent de repère opérationnel pour la défense et les migrations sensibles, dont la transition post-quantique.
- Alias: Agence nationale de la sécurité des systèmes d'information, French Cybersecurity Agency
- Voir aussi: `nist`, `fips`, `pqc`

### Backdoor
- ID: `backdoor`
- Catégorie: `cyber`
- Définition courte: Mécanisme caché permettant un accès non autorisé.
- Définition: Une backdoor peut être introduite dans du code, une dépendance ou un système pour maintenir un accès persistant en contournant les contrôles normaux.
- Alias: —
- Voir aussi: `supply-chain-attack`, `exfiltration`

### Blue Team
- ID: `blue-team`
- Catégorie: `cyber`
- Définition courte: Équipe défensive chargée de la prévention, détection et réponse.
- Définition: La Blue Team opère la surveillance, le durcissement, l'investigation et la réponse aux incidents pour réduire le risque dans la durée. Elle pilote les playbooks, la détection et l'amélioration continue des contrôles.
- Alias: équipe défensive, defensive security team
- Voir aussi: `soc`, `siem`, `xdr`

### C2
- ID: `c2`
- Catégorie: `cyber`
- Définition courte: Canal de Command and Control utilisé pour piloter un malware.
- Définition: Après compromission, un agent malveillant communique souvent avec un serveur C2 pour recevoir des ordres, exfiltrer des données ou pivoter.
- Alias: Command and Control, C&C
- Voir aussi: `ioc`, `ttp`

### CRQC
- ID: `crqc`
- Catégorie: `cyber`
- Définition courte: Ordinateur quantique capable de casser des schémas cryptographiques actuels.
- Définition: CRQC signifie Cryptographically Relevant Quantum Computer. Le terme désigne un seuil opérationnel: une machine quantique suffisamment stable et puissante pour menacer RSA et ECC à l'échelle réelle.
- Alias: Cryptographically Relevant Quantum Computer, ordinateur quantique cryptographiquement pertinent
- Voir aussi: `sndl`, `pqc`, `tls`

### CVE
- ID: `cve`
- Catégorie: `cyber`
- Définition courte: Identifiant standard public pour référencer une vulnérabilité connue.
- Définition: Le format CVE (Common Vulnerabilities and Exposures) permet de parler d’une faille avec une référence unique, utile pour le suivi et la remédiation.
- Alias: Common Vulnerabilities and Exposures
- Voir aussi: `zero-day`, `exploit`

### CVSS
- ID: `cvss`
- Catégorie: `cyber`
- Définition courte: Score standard pour évaluer la sévérité d'une vulnérabilité.
- Définition: Le Common Vulnerability Scoring System attribue une note (souvent sur 10) selon impact, exploitabilité et contexte, pour aider la priorisation.
- Alias: Common Vulnerability Scoring System
- Voir aussi: `cve`, `cwe`

### CWE
- ID: `cwe`
- Catégorie: `cyber`
- Définition courte: Classification des faiblesses logicielles communes.
- Définition: Common Weakness Enumeration décrit les types de failles de conception ou de développement et facilite la priorisation des corrections en amont.
- Alias: Common Weakness Enumeration
- Voir aussi: `cve`, `cvss`

### DLP
- ID: `dlp`
- Catégorie: `cyber`
- Définition courte: Contrôles empêchant la fuite de données sensibles.
- Définition: La Data Loss Prevention classe les données, applique des politiques (mail, endpoints, cloud) et bloque les exfiltrations non autorisées.
- Alias: Data Loss Prevention
- Voir aussi: `soc`, `zero-trust`

### Exfiltration
- ID: `exfiltration`
- Catégorie: `cyber`
- Définition courte: Extraction non autorisée de données hors d'un système.
- Définition: L'exfiltration suit souvent une compromission initiale: l'attaquant collecte puis transfère des données sensibles via un canal discret (C2, cloud, DNS, etc.).
- Alias: —
- Voir aussi: `c2`, `dlp`

### Exploit
- ID: `exploit`
- Catégorie: `cyber`
- Définition courte: Code ou technique qui tire parti d’une vulnérabilité.
- Définition: Un exploit transforme une faille théorique en impact concret: exécution de code, fuite de données, élévation de privilèges ou contournement de contrôles.
- Alias: —
- Voir aussi: `rce`, `zero-day`

### FIPS
- ID: `fips`
- Catégorie: `cyber`
- Définition courte: Normes fédérales américaines pour encadrer des mécanismes cryptographiques.
- Définition: Les Federal Information Processing Standards définissent des exigences techniques officielles. En post-quantique, FIPS 203, 204 et 205 cadrent ML-KEM, ML-DSA et SLH-DSA, et servent de référence pour les trajectoires de migration.
- Alias: Federal Information Processing Standards
- Voir aussi: `nist`, `ml-kem`, `ml-dsa`, `slh-dsa`

### IOC
- ID: `ioc`
- Catégorie: `cyber`
- Définition courte: Indicateur technique signalant une possible compromission.
- Définition: Les IOC incluent par exemple des hash, domaines, IP, URLs, patterns réseau ou artefacts système corrélés à des activités malveillantes.
- Alias: Indicator of Compromise, Indicateur de compromission
- Voir aussi: `siem`, `soc`

### MITRE ATLAS
- ID: `mitre-atlas`
- Catégorie: `cyber`
- Définition courte: Base de connaissances MITRE sur les techniques d'attaque ciblées IA.
- Définition: ATLAS documente tactiques, scénarios et mitigations pour les systèmes IA, dans une logique similaire à ATT&CK mais adaptée au contexte machine learning et agents.
- Alias: —
- Voir aussi: `ttp`, `prompt-injection`

### NIST
- ID: `nist`
- Catégorie: `cyber`
- Définition courte: Agence américaine de normalisation, référence technique en cybersécurité.
- Définition: Le National Institute of Standards and Technology publie des standards et guides largement utilisés pour la cryptographie, la sécurité des systèmes et la conformité. Ses publications structurent de nombreuses feuilles de route techniques.
- Alias: National Institute of Standards and Technology
- Voir aussi: `fips`, `pqc`, `ml-kem`

### OWASP
- ID: `owasp`
- Catégorie: `cyber`
- Définition courte: Fondation qui publie des standards et guides de sécurité applicative.
- Définition: L'Open Worldwide Application Security Project propose des référentiels utilisés pour auditer, prioriser et corriger les risques logiciels.
- Alias: Open Worldwide Application Security Project
- Voir aussi: `cwe`, `cve`

### Phishing
- ID: `phishing`
- Catégorie: `cyber`
- Définition courte: Technique d'ingénierie sociale visant à voler des identifiants ou donner accès.
- Définition: Le phishing imite une source légitime (mail, SMS, portail, voix) pour pousser la victime à cliquer, saisir ses secrets ou valider une action frauduleuse.
- Alias: —
- Voir aussi: `mfa`, `dmarc`

### Ransomware
- ID: `ransomware`
- Catégorie: `cyber`
- Définition courte: Malware qui chiffre les données et demande une rançon.
- Définition: Les campagnes modernes combinent chiffrement, vol de données et pression médiatique. La reprise dépend surtout des sauvegardes et du plan de réponse.
- Alias: rançongiciel
- Voir aussi: `c2`, `soc`

### RCE
- ID: `rce`
- Catégorie: `cyber`
- Définition courte: Exécution de code arbitraire à distance sur une cible.
- Définition: Une RCE est souvent critique car un attaquant peut faire exécuter des commandes sans accès local préalable.
- Alias: Remote Code Execution
- Voir aussi: `exploit`, `cve`

### SNDL
- ID: `sndl`
- Catégorie: `cyber`
- Définition courte: Risque de collecte chiffrée aujourd'hui pour déchiffrement futur.
- Définition: Store Now, Decrypt Later décrit la stratégie consistant à intercepter des flux chiffrés aujourd'hui pour les casser plus tard avec des capacités quantiques. Ce risque impose de traiter en priorité les données à forte durée de confidentialité.
- Alias: Store Now, Decrypt Later, collecter maintenant déchiffrer plus tard, harvest now decrypt later
- Voir aussi: `crqc`, `pqc`, `tls`

### Supply chain attack
- ID: `supply-chain-attack`
- Catégorie: `cyber`
- Définition courte: Attaque passant par un fournisseur, une dépendance ou un composant tiers.
- Définition: Au lieu de cibler directement l’entreprise finale, l’attaquant compromet la chaîne d’approvisionnement logicielle ou opérationnelle.
- Alias: attaque supply chain, attaque de la chaîne d’approvisionnement
- Voir aussi: `sbom`, `exploit`

### TTP
- ID: `ttp`
- Catégorie: `cyber`
- Définition courte: Tactiques, techniques et procédures utilisées par un acteur de menace.
- Définition: L’analyse TTP met l’accent sur les comportements adverses plutôt que sur un IOC isolé, utile pour une détection durable.
- Alias: Tactiques techniques procédures
- Voir aussi: `ioc`, `soc`

### YARA
- ID: `yara`
- Catégorie: `cyber`
- Définition courte: Langage de règles pour identifier des malwares et artefacts suspects.
- Définition: YARA permet d'écrire des signatures basées sur des motifs binaires, chaînes et conditions logiques, utiles en threat hunting et triage SOC.
- Alias: —
- Voir aussi: `ioc`, `soc`

### Zero-day
- ID: `zero-day`
- Catégorie: `cyber`
- Définition courte: Vulnérabilité exploitée avant qu’un correctif officiel ne soit disponible.
- Définition: Un zero-day crée une fenêtre de risque maximale: l’attaque est possible pendant que les défenseurs n’ont pas encore de patch stable à déployer.
- Alias: 0-day, zero day
- Voir aussi: `cve`, `exploit`

## IA & Agents

### Agent IA
- ID: `ai-agent`
- Catégorie: `ai`
- Définition courte: Système IA capable d’appeler des outils et d’exécuter des actions.
- Définition: Un agent IA combine raisonnement, mémoire, contexte et exécution opérationnelle. Son périmètre doit être strictement borné.
- Alias: AI agent, agentic AI
- Voir aussi: `mcp`, `prompt-injection`, `sandboxing`

### Data poisoning
- ID: `data-poisoning`
- Catégorie: `ai`
- Définition courte: Injection de données malicieuses pour biaiser un modèle.
- Définition: Le poisoning peut toucher pre-training, fine-tuning ou index RAG et conduire à des réponses manipulées, portes dérobées logiques ou décisions dégradées.
- Alias: empoisonnement de données
- Voir aussi: `rag`, `backdoor`

### Deepfake
- ID: `deepfake`
- Catégorie: `ai`
- Définition courte: Média synthétique généré par IA imitant une personne réelle.
- Définition: Les deepfakes audio/video servent à tromper une cible (fraude, désinformation, usurpation) et augmentent fortement le risque de phishing avancé.
- Alias: —
- Voir aussi: `phishing`

### Jailbreak LLM
- ID: `jailbreak-llm`
- Catégorie: `ai`
- Définition courte: Tentative de contourner les garde-fous d’un modèle.
- Définition: Le jailbreak vise à obtenir des réponses interdites via reformulation, rôle fictif, obfuscation ou chaînage d’instructions.
- Alias: LLM jailbreak
- Voir aussi: `prompt-injection`

### MCP
- ID: `mcp`
- Catégorie: `ai`
- Définition courte: Model Context Protocol: standard d’intégration outils et contexte pour LLM.
- Définition: MCP normalise la façon dont un agent découvre des outils, lit du contexte et lance des actions, en réduisant le couplage propriétaire.
- Alias: Model Context Protocol
- Voir aussi: `ai-agent`, `sandboxing`

### Prompt injection
- ID: `prompt-injection`
- Catégorie: `ai`
- Définition courte: Technique qui manipule un LLM via des instructions malicieuses.
- Définition: Un contenu externe (page web, email, document) peut injecter des consignes qui contournent les règles attendues du modèle.
- Alias: injection de prompt
- Voir aussi: `jailbreak-llm`, `ai-agent`

### RAG
- ID: `rag`
- Catégorie: `ai`
- Définition courte: Approche qui combine recherche documentaire et génération par LLM.
- Définition: Retrieval-Augmented Generation injecte du contexte externe (base documentaire, wiki, logs) au moment de la réponse pour réduire les hallucinations et ancrer les sorties.
- Alias: Retrieval-Augmented Generation
- Voir aussi: `mcp`, `data-poisoning`

## Infra & Ops

### DMARC
- ID: `dmarc`
- Catégorie: `infra`
- Définition courte: Politique email anti-usurpation basée sur SPF et DKIM.
- Définition: DMARC définit comment traiter les emails non alignés (none, quarantine, reject) et fournit des rapports pour piloter la protection du domaine.
- Alias: Domain-based Message Authentication, Reporting and Conformance
- Voir aussi: `phishing`

### ECDH
- ID: `ecdh`
- Catégorie: `infra`
- Définition courte: Mécanisme d'échange de clé basé sur les courbes elliptiques.
- Définition: Elliptic Curve Diffie-Hellman permet à deux parties d'établir un secret partagé pour initialiser des sessions chiffrées. En transition post-quantique, il est souvent combiné à ML-KEM dans des schémas hybrides.
- Alias: Elliptic Curve Diffie-Hellman
- Voir aussi: `ecdsa`, `rsa`, `ml-kem`, `tls`

### ECDSA
- ID: `ecdsa`
- Catégorie: `infra`
- Définition courte: Schéma de signature numérique basé sur les courbes elliptiques.
- Définition: Elliptic Curve Digital Signature Algorithm est utilisé pour authentifier certificats et échanges signés. Dans les migrations PQC, il est progressivement complété par ML-DSA ou SLH-DSA.
- Alias: Elliptic Curve Digital Signature Algorithm
- Voir aussi: `ecdh`, `rsa`, `ml-dsa`, `slh-dsa`

### EDR
- ID: `edr`
- Catégorie: `infra`
- Définition courte: Détection et réponse sur endpoints.
- Définition: Un EDR collecte la télémétrie poste/serveur, détecte des comportements suspects et assiste l'investigation et la remédiation en temps réel.
- Alias: Endpoint Detection and Response
- Voir aussi: `xdr`, `soc`

### HKDF
- ID: `hkdf`
- Catégorie: `infra`
- Définition courte: Fonction de dérivation HMAC utilisée dans les schedules TLS 1.3.
- Définition: HKDF applique un schéma extract-then-expand pour dériver des clés robustes à partir d'un secret initial. Cette primitive est centrale dans TLS 1.3 et dans plusieurs constructions hybrides.
- Alias: HMAC-based Key Derivation Function
- Voir aussi: `kdf`, `tls`, `kem`

### HSM
- ID: `hsm`
- Catégorie: `infra`
- Définition courte: Module matériel protégé pour stocker et utiliser des clés.
- Définition: Un Hardware Security Module exécute des opérations cryptographiques sensibles dans un environnement durci. Les capacités HSM déterminent souvent le rythme de modernisation d'une PKI et la migration post-quantique.
- Alias: Hardware Security Module
- Voir aussi: `pki`, `ml-dsa`, `slh-dsa`

### IAM
- ID: `iam`
- Catégorie: `infra`
- Définition courte: Gestion des identités et des droits d'accès.
- Définition: IAM structure comptes, rôles, policies et fédération pour appliquer moindre privilège, traçabilité et contrôle fin des permissions.
- Alias: Identity and Access Management
- Voir aussi: `zero-trust`, `mfa`

### KDF
- ID: `kdf`
- Catégorie: `infra`
- Définition courte: Fonction qui dérive des clés à partir d'un secret initial.
- Définition: Une Key Derivation Function transforme un secret partagé en plusieurs clés adaptées à des usages distincts. Elle est incontournable pour les protocoles modernes et les combinaisons cryptographiques hybrides.
- Alias: Key Derivation Function
- Voir aussi: `hkdf`, `kem`, `tls`

### KEM
- ID: `kem`
- Catégorie: `infra`
- Définition courte: Mécanisme d'encapsulation de clé pour établir un secret partagé.
- Définition: Un Key Encapsulation Mechanism permet de construire un secret commun via encapsulation puis décapsulation. Il est essentiel dans les protocoles post-quantiques et dans les architectures de transition hybrides.
- Alias: Key Encapsulation Mechanism
- Voir aussi: `ml-kem`, `kdf`, `tls`

### MFA
- ID: `mfa`
- Catégorie: `infra`
- Définition courte: Authentification avec plusieurs facteurs indépendants.
- Définition: La MFA combine au moins deux preuves (mot de passe, appareil, biométrie, clé physique) pour réduire le risque de compromission de compte.
- Alias: authentification multifacteur
- Voir aussi: `iam`, `phishing`

### ML-DSA
- ID: `ml-dsa`
- Catégorie: `infra`
- Définition courte: Standard NIST de signature numérique post-quantique basé sur réseaux.
- Définition: ML-DSA (FIPS 204) fournit un schéma de signature post-quantique orienté performances et déploiement opérationnel. Il est utilisé pour signer des certificats, artefacts logiciels et échanges nécessitant une authentification forte.
- Alias: FIPS 204, Dilithium
- Voir aussi: `pqc`, `ml-kem`, `slh-dsa`

### ML-KEM
- ID: `ml-kem`
- Catégorie: `infra`
- Définition courte: Standard NIST de KEM post-quantique pour établir des clés partagées.
- Définition: ML-KEM (FIPS 203) est un mécanisme d'encapsulation de clé basé sur les réseaux. Il est destiné à des usages comme TLS, VPN ou SSH pour l'établissement de clé résistant aux attaques quantiques.
- Alias: FIPS 203, Kyber
- Voir aussi: `pqc`, `ml-dsa`, `tls`

### PKI
- ID: `pki`
- Catégorie: `infra`
- Définition courte: Infrastructure de gestion des certificats et des clés publiques.
- Définition: La Public Key Infrastructure gère émission, rotation, révocation et validation des certificats. Elle constitue un pivot technique pour déployer de nouvelles signatures et maintenir la confiance dans les systèmes distribués.
- Alias: Public Key Infrastructure
- Voir aussi: `hsm`, `ml-dsa`, `slh-dsa`, `tls`

### PQC
- ID: `pqc`
- Catégorie: `infra`
- Définition courte: Cryptographie conçue pour résister aux attaques d'ordinateurs quantiques.
- Définition: La cryptographie post-quantique remplace ou complète les algorithmes asymétriques vulnérables à Shor. En pratique, la transition passe souvent par des déploiements hybrides, puis une adoption progressive des standards normalisés.
- Alias: cryptographie post-quantique, post-quantum cryptography
- Voir aussi: `ml-kem`, `ml-dsa`, `slh-dsa`, `tls`

### RSA
- ID: `rsa`
- Catégorie: `infra`
- Définition courte: Algorithme asymétrique historique pour chiffrement et signatures.
- Définition: RSA reste très déployé dans les systèmes hérités et certaines PKI. Son exposition théorique aux attaques quantiques en fait une cible prioritaire dans les plans de transition vers des mécanismes post-quantiques.
- Alias: —
- Voir aussi: `ecdh`, `ecdsa`, `pqc`

### Sandboxing
- ID: `sandboxing`
- Catégorie: `infra`
- Définition courte: Isolation contrôlée pour limiter l’impact d’un code non fiable.
- Définition: Une sandbox limite permissions, système de fichiers, réseau et appels système pour contenir un comportement malveillant.
- Alias: bac à sable, sandbox
- Voir aussi: `ai-agent`, `zero-trust`

### SIEM
- ID: `siem`
- Catégorie: `infra`
- Définition courte: Plateforme centralisant logs, corrélations et alertes sécurité.
- Définition: Le SIEM agrège les événements de multiples sources et applique des règles pour détecter des comportements anormaux.
- Alias: Security Information and Event Management
- Voir aussi: `soc`, `ioc`, `ttp`

### SLH-DSA
- ID: `slh-dsa`
- Catégorie: `infra`
- Définition courte: Standard NIST de signature post-quantique basé sur fonctions de hachage.
- Définition: SLH-DSA (FIPS 205) est un schéma de signature stateless basé sur le hachage. Il apporte une alternative à ML-DSA avec des hypothèses différentes, utile pour diversifier les choix cryptographiques.
- Alias: FIPS 205, SPHINCS+
- Voir aussi: `pqc`, `ml-dsa`

### SOC
- ID: `soc`
- Catégorie: `infra`
- Définition courte: Équipe opérationnelle de surveillance et réponse incidents.
- Définition: Le Security Operations Center supervise la détection, qualification, investigation et remédiation des incidents de sécurité.
- Alias: Security Operations Center
- Voir aussi: `siem`, `ioc`, `ttp`

### SSH
- ID: `ssh`
- Catégorie: `infra`
- Définition courte: Protocole sécurisé pour accès distant, transfert et tunnels.
- Définition: Secure Shell protège les sessions d'administration et les transferts via chiffrement et authentification. Sa migration post-quantique dépend des extensions supportées par clients, serveurs et équipements intermédiaires.
- Alias: Secure Shell
- Voir aussi: `tls`, `vpn`, `pqc`

### TLS
- ID: `tls`
- Catégorie: `infra`
- Définition courte: Protocole de chiffrement des communications réseau.
- Définition: Transport Layer Security protège la confidentialité et l'intégrité des flux (HTTPS, API, mail) via chiffrement, certificats et négociation cryptographique.
- Alias: Transport Layer Security
- Voir aussi: `zero-trust`

### VPN
- ID: `vpn`
- Catégorie: `infra`
- Définition courte: Tunnel chiffré reliant des utilisateurs ou réseaux distants.
- Définition: Un Virtual Private Network sécurise les communications inter-sites ou nomades sur des réseaux non fiables. La compatibilité des suites cryptographiques et des appliances est un facteur clé de migration.
- Alias: Virtual Private Network
- Voir aussi: `tls`, `ssh`, `pqc`

### WAF
- ID: `waf`
- Catégorie: `infra`
- Définition courte: Pare-feu applicatif web filtrant le trafic HTTP(S).
- Définition: Un WAF bloque ou limite des patterns d’attaque applicative (SQLi, XSS, bots), avec règles gérées ou personnalisées.
- Alias: Web Application Firewall
- Voir aussi: `zero-trust`, `siem`

### XDR
- ID: `xdr`
- Catégorie: `infra`
- Définition courte: Détection et réponse étendues sur plusieurs couches.
- Définition: Le XDR corrèle endpoints, réseau, email, cloud et identité pour accélérer la détection multi-source et la réponse coordonnée.
- Alias: Extended Detection and Response
- Voir aussi: `edr`, `siem`

### Zero Trust
- ID: `zero-trust`
- Catégorie: `infra`
- Définition courte: Principe: ne jamais faire confiance par défaut, toujours vérifier.
- Définition: Le modèle Zero Trust applique vérification continue, moindre privilège et segmentation forte, même dans le réseau interne.
- Alias: zéro confiance
- Voir aussi: `sandboxing`, `soc`

## Dev & Architecture

### CI/CD
- ID: `ci-cd`
- Catégorie: `dev`
- Définition courte: Pipeline automatisé de build, test et déploiement.
- Définition: La Continuous Integration et la Continuous Delivery/Deployment réduisent les délais de mise en production, mais imposent un durcissement fort de la supply chain logicielle.
- Alias: Continuous Integration, Continuous Delivery, Continuous Deployment
- Voir aussi: `sbom`, `supply-chain-attack`

### Crypto-agilité
- ID: `crypto-agility`
- Catégorie: `dev`
- Définition courte: Capacité d'un système à changer d'algorithmes cryptographiques sans refonte majeure.
- Définition: La crypto-agilité repose sur des abstractions, paramètres configurables et stratégies de migration maîtrisées. Elle limite l'effet tunnel lors des transitions, notamment vers la cryptographie post-quantique.
- Alias: agilité cryptographique, cryptographic agility
- Voir aussi: `pqc`, `tls`, `ci-cd`

### JWT
- ID: `jwt`
- Catégorie: `dev`
- Définition courte: Jeton signé pour transporter des claims d'authentification/autorisation.
- Définition: JSON Web Token permet de propager l'identité et des droits entre services. La sécurité dépend de la signature, de la rotation des clés, de l'expiration et des contrôles côté serveur.
- Alias: JSON Web Token
- Voir aussi: `iam`, `mfa`

### RSC
- ID: `rsc`
- Catégorie: `dev`
- Définition courte: React Server Components: rendu et logique exécutée côté serveur.
- Définition: RSC déplace une partie du rendu React côté serveur pour réduire le JavaScript client, mais introduit aussi des enjeux de sécurité autour de la sérialisation et des frontières serveur/client.
- Alias: React Server Components
- Voir aussi: `rce`, `cve`

### SBOM
- ID: `sbom`
- Catégorie: `dev`
- Définition courte: Inventaire des composants logiciels d’une application.
- Définition: Le SBOM (Software Bill of Materials) améliore la visibilité sur les dépendances et facilite l’évaluation d’impact lors d’une CVE.
- Alias: Software Bill of Materials
- Voir aussi: `supply-chain-attack`, `cve`

