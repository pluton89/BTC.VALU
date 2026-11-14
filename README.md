# BTC/EUR Live Terminal & Bot Discord Automatique

## Contenu du pack
1. `index.html` : Ton site web complet (sans ton webhook exposé en clair dans le code).
2. `.github/workflows/auto-discord.yml` : Le robot GitHub Actions qui ouvre ton site toutes les 30 minutes et envoie le prix, les pourcentages et la photo du graphique sur Discord.

## Installation sur GitHub (3 minutes)
1. Crée un dépôt sur GitHub (ex: `btc-discord-tracker`).
2. Dépose les fichiers de cette archive dedans (en conservant bien le dossier `.github/workflows/auto-discord.yml`).
3. Va dans **Settings > Secrets and variables > Actions** > **New repository secret** :
   - **Name** : `DISCORD_WEBHOOK`
   - **Secret** : Colle ton URL de webhook Discord.
4. (Optionnel) Pour avoir ton site accessible en ligne : va dans **Settings > Pages**, choisis la branche `main` et clique sur **Save**.
5. Pour tester immédiatement : va dans l'onglet **Actions** de ton dépôt GitHub, clique sur **Envoi Graphique BTC Discord** puis sur **Run workflow**.
