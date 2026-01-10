# Outil de Test de Sécurité Yahoo avec IA Avancée | À des Fins Éducatives Uniquement

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![IA](https://img.shields.io/badge/IA-Activée-brightgreen)
![Sécurité](https://img.shields.io/badge/Sécurité-Audit-red)
![Licence](https://img.shields.io/badge/Licence-Éducative%20Uniquement-lightgreen)

---

## AVIS JURIDIQUE – LISEZ ATTENTIVEMENT

Ce projet est strictement destiné à l'ÉDUCATION, à la RECHERCHE et aux TESTS DE SÉCURITÉ AUTORISÉS.

### AVERTISSEMENT IMPORTANT

- **Utilisation non autorisée interdite** : Toute tentative d'accès à des comptes Yahoo sans autorisation explicite est illégale.
- **Autorisation requise** : Les tests ne peuvent être effectués que sur des comptes que vous possédez ou pour lesquels vous avez une autorisation écrite.
- **But éducatif** : Ce projet vise à démontrer les vulnérabilités de sécurité potentielles et à promouvoir de meilleures pratiques de sécurité.
- **Responsabilité** : L'utilisateur est seul responsable du respect des lois et réglementations en vigueur.

En utilisant ce logiciel, vous reconnaissez que l'accès non autorisé aux systèmes informatiques est un délit pénal dans de nombreuses juridictions.

**J'ai utilisé l'API de PASS REVELATOR pour créer ce programme, et je les remercie pour leur soutien. Si vous souhaitez en savoir plus sur la sécurité des comptes Yahoo et le piratage des mots de passe, je vous invite à visiter leur site web : https://www.passwordrevelator.net/fr/passaccess**

![PASSACCESS_Logo](./PASSACCESS.webp)

---

## Aperçu du Projet

L'outil de Test de Sécurité Yahoo avec IA est une solution avancée de cybersécurité conçue pour démontrer comment l'IA peut être utilisée pour pirater des mots de passe. Cet outil intègre des techniques d'apprentissage automatique pour tester la sécurité des comptes Yahoo de manière intelligente.

### Objectifs Pédagogiques

- Démontrer les techniques modernes d'analyse de sécurité avec l'IA
- Sensibiliser aux risques liés aux mots de passe faibles
- Fournir un outil éducatif pour les professionnels de la cybersécurité
- Explorer les mécanismes de défense contre les attaques automatisées
- Comprendre l'importance des politiques de mots de passe robustes

### Fonctionnalités Principales

#### Intelligence Artificielle Avancée
- Génération de mots de passe basée sur les chaînes de Markov
- Réseaux de neurones LSTM pour la prédiction de séquences
- Apprentissage par renforcement pour améliorer les stratégies d'attaque
- Détection des modèles de mots de passe courants

#### Sécurité et Anonymat
- Support complet du réseau Tor pour l'anonymat
- Rotation intelligente des proxies
- Délais aléatoires entre les requêtes
- Gestion avancée des sessions et des cookies

#### Analyse et Rapports
- Suivi en temps réel des tentatives
- Statistiques détaillées de performance
- Génération de rapports complets
- Journalisation avancée des opérations

#### Performances
- Architecture asynchrone pour des performances élevées
- Gestion efficace de la mémoire
- Support multi-thread
- Optimisation des requêtes réseau

---

## Guide d'Installation

### Prérequis

- Python 3.8 ou supérieur
- Gestionnaire de paquets pip
- Connexion Internet active
- Compte développeur Yahoo (pour les tests autorisés)

### Étape 1 : Cloner le Dépôt

```bash
git clone https://github.com/HoffmannAlex/Hack-Yahoo-Account-with-AI.git
cd yahoo-security-tool
```

### Étape 2 : Créer un environnement virtuel (Recommandé)

```bash
python -m venv venv
source venv/bin/activate  # Sur Linux/Mac
# OU
.\venv\Scripts\activate  # Sur Windows
```

### Étape 3 : Installer les Dépendances

```bash
pip install -r requirements.txt
```

### Dépendances Principales

- aiohttp>=3.9.1
- requests>=2.31.0
- cryptography>=42.0.5
- psutil>=5.9.8
- asyncio>=3.4.3
- python-dotenv>=1.0.1
- msal>=1.24.1
- markovify>=0.9.4
- numpy>=1.24.3
- python-jose>=3.3.0

### Étape 4 : Configuration Initiale

1. Copiez le fichier de configuration exemple :
   ```bash
   cp config.example.json config.json
   ```

2. Modifiez le fichier `config.json` selon vos besoins :
   ```json
   {
       "max_attempts": 1000,
       "delay_range": [1.0, 3.0],
       "timeout": 3600,
       "results_file": "security_results.json",
       "proxy_file": "proxies.txt",
       "use_tor": false,
       "verbose": false
   }
   ```

### Étape 5 : Vérifier l'Installation

```bash
python hack_yahoo.py --help
```

---

## Exemples d'Utilisation

### Test de Sécurité de Base

```bash
# Exécuter un test de sécurité avec la configuration par défaut
python hack_yahoo.py --username utilisateur@yahoo.com

# Spécifier un fichier de configuration personnalisé
python hack_yahoo.py --username utilisateur@yahoo.com --config config_perso.json
```

### Options d'Anonymat et de Confidentialité

```bash
# Utiliser le réseau Tor pour l'anonymat
python hack_yahoo.py --username utilisateur@yahoo.com --use-tor

# Utiliser une liste de proxies personnalisée
python hack_yahoo.py --username utilisateur@yahoo.com --proxy-list proxies.txt
```

### Contrôle des Performances

```bash
# Définir le nombre maximal de tentatives
python hack_yahoo.py --username utilisateur@yahoo.com --max-attempts 500

# Définir des délais personnalisés entre les tentatives (en secondes)
python hack_yahoo.py --username utilisateur@yahoo.com --min-delay 2.0 --max-delay 5.0

# Activer le mode verbeux pour plus de détails
python hack_yahoo.py --username utilisateur@yahoo.com --verbose
```

### Gestion des Résultats

```bash
# Spécifier un fichier de sortie personnalisé
python hack_yahoo.py --username utilisateur@yahoo.com --output resultats/audit_2026.json

# Reprendre un test précédent à partir d'un fichier de résultats
python hack_yahoo.py --resume resultats/audit_2026.json
```

---

## Configuration Avancée

### Fichier de Configuration (config.json)

```json
{
    "max_attempts": 1000,
    "delay_range": [1.0, 3.0],
    "timeout": 3600,
    "results_file": "security_results.json",
    "proxy_file": "proxies.txt",
    "use_tor": false,
    "tor_port": 9050,
    "tor_control_port": 9051,
    "tor_password": "votre_mot_de_passe_tor",
    "user_agents": [
        "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
        "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:89.0) Gecko/20100101 Firefox/89.0"
    ],
    "log_level": "INFO",
    "log_file": "yahoo_security_test.log"
}
```

### Variables d'Environnement

Vous pouvez également configurer l'application en utilisant des variables d'environnement :

```bash
export YAHOO_USERNAME=utilisateur@yahoo.com
export YAHOO_MAX_ATTEMPTS=1000
export YAHOO_USE_TOR=true
python hack_yahoo.py
```

---

## Dépannage

### Problèmes Courants

1. **Erreur de Connexion**
   - Vérifiez votre connexion Internet
   - Si vous utilisez un proxy ou Tor, assurez-vous qu'il est correctement configuré

2. **Limitation de Débit**
   - Augmentez les délais entre les requêtes avec `--min-delay` et `--max-delay`
   - Utilisez `--use-tor` pour éviter les restrictions basées sur l'IP

3. **Erreurs d'Authentification**
   - Vérifiez que le nom d'utilisateur est correct
   - Assurez-vous d'avoir les autorisations nécessaires

### Journaux et Débogage

Les journaux sont enregistrés dans `yahoo_security_test.log` par défaut. Pour un débogage plus approfondi :

```bash
python hack_yahoo.py --username utilisateur@yahoo.com --log-level DEBUG
```

---

## Considérations Légales et Éthiques

### Avertissement Légal

Cet outil est fourni uniquement à des fins éducatives et de test de sécurité autorisé. Les développeurs déclinent toute responsabilité quant à l'utilisation abusive de ce logiciel ou aux dommages qu'il pourrait causer. L'utilisateur final est seul responsable du respect de toutes les lois locales, nationales et fédérales applicables.

### Directives d'Utilisation Éthique

1. **Autorisation** : Ne testez que les comptes que vous possédez ou pour lesquels vous avez une autorisation écrite explicite.
2. **Conformité Légale** : Respectez toutes les lois sur la cybersécurité et la protection des données en vigueur dans votre juridiction.
3. **Responsabilité** : Vous êtes seul responsable de l'utilisation de cet outil et de ses conséquences.
4. **Sécurité** : Ne stockez jamais de mots de passe ou d'informations sensibles en clair.

### Déclaration de Conformité

En utilisant cet outil, vous reconnaissez que :
- L'accès non autorisé aux systèmes informatiques est illégal dans la plupart des juridictions.
- Toute activité malveillante peut entraîner des poursuites pénales.
- Les résultats des tests doivent être utilisés uniquement pour améliorer la sécurité des systèmes concernés.

---

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

## Remerciements

- Aux contributeurs du projet pour leur travail acharné
- À la communauté open source pour ses précieuses ressources
- Aux chercheurs en sécurité qui partagent leurs connaissances

## Contribution

Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une issue ou à soumettre une pull request.

## Contact

Pour toute question ou préoccupation, veuillez ouvrir une issue sur GitHub.
