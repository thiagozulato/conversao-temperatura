FROM node:17-alpine

LABEL iniciativa="KubeDev"

WORKDIR /app

# Aqui copia apenas o json para manter o cache da imagem, pois somente será compilado novamente quando o mesmo mudar.
COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 8080

ENTRYPOINT ["node", "server.js"]
