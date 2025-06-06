# recover node image from dockhub, version is specified
FROM node:22.11.0

# define the working directory inside the contener as being /app. The app will lives here
WORKDIR /app

# copy all the package.json from the current directory
COPY package*.json ./

# run the npm install command to install all dependencies BEFORE copying the app files
RUN npm install

# copy all the app files in the container
COPY . .

#a command to run the container once everything else is done
CMD ["npm", "run", "dev"]