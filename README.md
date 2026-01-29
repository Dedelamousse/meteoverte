# 🌤️ Météo Verte - Application Météo

Application météo simple et élégante utilisant l'API OpenWeatherMap.

## 🔐 Configuration Sécurisée

### Étape 1 : Configurer le Secret GitHub

1. Allez dans votre repository GitHub : `https://github.com/Dedelamousse/meteoverte`
2. Cliquez sur **Settings** (Paramètres)
3. Dans le menu de gauche, cliquez sur **Secrets and variables** → **Actions**
4. Cliquez sur **New repository secret**
5. Configurez le secret :
   - **Name** : `OPENWEATHER_API_KEY`
   - **Value** : Collez votre nouvelle clé API OpenWeatherMap
6. Cliquez sur **Add secret**

### Étape 2 : Activer GitHub Pages avec Actions

1. Allez dans **Settings** → **Pages**
2. Dans **Source**, sélectionnez **GitHub Actions**
3. Sauvegardez

### Étape 3 : Déployer

1. Remplacez votre fichier `index.html` actuel par le nouveau fichier sécurisé
2. Ajoutez le dossier `.github/workflows/` avec le fichier `deploy.yml`
3. Commitez et poussez les changements :
   ```bash
   git add .
   git commit -m "Secure API key using GitHub Secrets"
   git push
   ```

Le déploiement se fera automatiquement et votre clé API sera injectée de manière sécurisée !

## 🚀 Fonctionnalités

- ✅ Recherche de météo par ville
- ✅ Affichage de la température actuelle
- ✅ Humidité, vitesse du vent, et température ressentie
- ✅ Interface responsive et moderne
- ✅ Clé API sécurisée

## 📝 Notes de Sécurité

⚠️ **Important** : Ne jamais commiter de clés API directement dans le code !

- ✅ Les clés sont stockées dans les secrets GitHub
- ✅ Elles sont injectées automatiquement lors du déploiement
- ✅ Le code source ne contient que des placeholders

## 🌐 Accès à l'Application

Une fois déployée, l'application sera accessible à :
`https://dedelamousse.github.io/meteoverte/`
