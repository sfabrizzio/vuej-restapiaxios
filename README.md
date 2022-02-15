Vue.js (comúnmente conocido como Vue; se pronuncia /vjuː/, como "view"3​) es un framework de JavaScript de código abierto para la construcción de interfaces de usuario y aplicaciones 

# EJEMPLO BASICO CRUD CON VUE.JS Y AXIOS EMPLEANDO SERVICE

# EN ESTE EJEMPLO SE UTILIZA VUETIFY es un marco de interfaz de usuario completo construido sobre Vue.js. 
## Project setup
```
Instalación del servidor JSON
JSON Server está disponible como paquete NPM. La instalación se puede realizar utilizando el administrador de paquetes Node.js:
npm install -g json-server

Pimero ejecutar :
npm install
```
luego :

npm run serve

### APÌ REST LOCAL
```

``
# Se Añadiò  una base de datos local creando un archivo bd.json con algunos datos. En este caso vamos a añadir algunos datoss:

{
    "frameworks": [
      {
        "id": 1,
        "name": "React"
      },
      {
        "id": 2,
        "name": "Vuejs"
      },
      {
        "id": 3,
        "name": "Angular"
      }
    ]
  }`
  
  
# en un nuevo terminal , digitar :
json-server --watch src/data_base/bd.json

para Obtener una API REST falsa completa sin codificación 
# http://localhost:3000/frameworks
### Compiles and minifies for production
```

![image](https://user-images.githubusercontent.com/15172436/149638363-1a90681b-c22f-4e63-8a2d-967ca1199dfc.png)

npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
echo "# vuerjs-vuetify-axios2" 
