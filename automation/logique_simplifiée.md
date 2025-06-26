# 🔄 Logique simplifiée du système

Ce projet repose sur un scénario Make entièrement automatisé, qui transforme un brief client en logo généré par IA, sans intervention manuelle.

---

## 🧩 Grandes étapes du processus

1. **Formulaire rempli par le client (Tally)**  
   Le client fournit les éléments du brief : nom, slogan, style, couleurs, etc.

2. **Déclenchement automatique (Webhook Make)**  
   Dès validation du formulaire, le scénario se lance automatiquement.

3. **Traitement des données (Make)**  
   Les réponses sont nettoyées, formatées, et les styles choisis sont traduits en texte lisible.

4. **Génération d’un prompt (ChatGPT via API)**  
   Un prompt clair et professionnel est généré à partir des réponses du client.

5. **Création du logo (DALL·E)**  
   Le prompt est transmis à DALL·E pour générer une ou plusieurs propositions de logo.

6. **Sauvegardes (Dropbox + Google Sheets)**  
   Les données du brief, les prompts et les visuels sont enregistrés automatiquement :
   - sur Dropbox (fichiers)
   - dans Google Sheets (données et suivi)

7. **Envoi par e-mail (Make SMTP)**  
   Un e-mail est envoyé automatiquement avec les résultats (brief, prompt, ou image).

---

💡 Ce projet m’a permis de me familiariser avec l’automatisation no-code, l’API d’OpenAI, la gestion de données JSON, et l’orchestration entre plusieurs services (Tally, Dropbox, Google Sheets, SMTP).
