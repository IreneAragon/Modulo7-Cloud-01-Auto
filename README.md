# Ejercicio 1 - Github Pages - Automatizado 
He tomado el último ejercicio del máster y he realizado en él los cambios necesarios para subir el proyecto a Github Pages de forma automatizada.

## Pasos que he seguido: 
1. Instalar la librería `gh-pages`
```bash
npm install gh-pages -D
```
2. Congifurar los comandos para usar la librería en  `package.json`, 
`"build:dev": "npm run clean && webpack --config ./config/webpack/dev.js"`
`"deploy": "gh-pages -d dist"`
3. Al ejecutar el comando `npm run build:dev` se genera la carpeta dist de modo desarrollo y al ejecutar el comando `npm run deploy` automáticamente se crea la rama `gh-pages` y se suben los archivos de la carpeta `dist`sin nosotros tener que hacer nada, es automático. 
```bash
npm run build:dev
npm run deploy
```