# Utiliser une image Node.js Alpine
FROM node:current-alpine3.16

# Créer et définir le répertoire de travail de l'application dans l'image
WORKDIR /usr/src/app

# Copier les fichiers du projet dans l'image
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier le reste des fichiers de l'application
COPY . .

# Exposer le port sur lequel l'application s'exécute
EXPOSE 3000

# Commande pour démarrer l'application
CMD ["npm", "start"]

