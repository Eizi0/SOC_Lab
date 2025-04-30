# 🛡️ SOC_Lab for Blue Team (Wazuh, Suricata, Sigma, MISP, YARA)

Bienvenue dans **SOC_Lab**, un environnement de simulation SOC orienté Blue Team, conçu pour apprendre, tester et expérimenter la détection et la réponse aux incidents de sécurité.

## 🎯 Objectifs

- Créer un lab complet pour la surveillance, la détection et le threat hunting
- Centraliser et corréler des logs via Wazuh et l’ELK Stack
- Détecter des attaques réseau et système grâce à Suricata, Sigma, YARA
- Intégrer des sources de threat intelligence avec MISP
- Simuler des attaques sur des machines cibles pour valider la détection

## 🧱 Architecture technique

| Rôle            | Outils                          | Description                                      |
|-----------------|----------------------------------|--------------------------------------------------|
| SOC / SIEM      | Wazuh, ELK Stack                | Centralisation des logs, génération d’alertes    |
| IDS réseau      | Suricata                        | Détection en temps réel du trafic réseau         |
| Threat Intel    | MISP                            | Base IoC, corrélation avec les événements        |
| Détection       | Sigma, YARA                     | Règles personnalisées pour logs et fichiers      |
| Machine cible   | Windows / Linux vulnérables     | Simuler des compromissions                      |
| Machine RedTeam | Kali Linux / Parrot OS          | Exécution de scénarios d’attaque                 |
| Dashboards      | Grafana / Kibana                | Visualisation des données et alertes             |

📌 Le lab repose sur **Proxmox VE** pour la gestion des VM, mais peut être adapté à VirtualBox ou VMware.

## ⚙️ Composants à déployer

- [ ] Proxmox + Réseau virtuel
- [ ] VM Wazuh Manager (avec ELK)
- [ ] VM OPNSense + Suricata (mode IDS)
- [ ] VM MISP + intégration avec Wazuh
- [ ] Règles Sigma + YARA personnalisées
- [ ] VM Windows/Linux vulnérable
- [ ] Attaques simulées (brute force, phishing, malware…)

## 🔍 Scénarios prévus

1. **Détection de brute force SSH avec Suricata + Wazuh**
2. **Téléchargement de malware – détection via YARA**
3. **Corrélation d’IoC issu de MISP dans les logs**
4. **Alertes multiples sur mouvement latéral ou exfiltration**

## 🧠 Prérequis

- Connaissances de base en Linux, réseau, et cybersécurité
- Un serveur Proxmox (ou équivalent) avec au moins 32 Go RAM
- (Recommandé) Connexion avec accès Internet pour les MAJ et CTI

## 📊 Capture d’écran / Dashboards

*(À venir – captures Kibana, Grafana, alertes Wazuh, logs Suricata…)*

## 📚 Liens utiles

- [https://wazuh.com/](https://wazuh.com/)
- [https://suricata.io/](https://suricata.io/)
- [https://www.misp-project.org/](https://www.misp-project.org/)
- [https://sigmahq.io/](https://sigmahq.io/)
- [https://yara.readthedocs.io/](https://yara.readthedocs.io/)
- [https://www.proxmox.com/](https://www.proxmox.com/)

## 👤 Auteur

**Jeovany N.**  
Étudiant en Mastère Cybersécurité 
Passionné par la détection des menaces, les SOC et la cyberdéfense

📧 Contact : [ton email pro ici]  
📅 Disponible pour une alternance en cybersécurité dès octobre 2025

---

> 📌 Ce projet est en développement actif. Contributions, suggestions et remarques sont les bienvenues !
