#Conectar a nuestro contenedodor docker que se esta corriendo
#OJO:Nombre del servicio es mongodb, ese servicio esrta en el archivo docker-compose.yml

#Connect to container
``````sh
docker-compose exec mongodb bash
`````

# Connect with mongosh (This conect our database with the terminal of mongo to start querying o doing whatever I want)

`````sh
mongosh "mongodb://root:root123@localhost:27017/?authMechanism=DEFAULT&tls=false"
mongosh "mongodb+srv://clavijoadmin:clavijo123@mongodb101.jaq3out.mongodb.net/"
`````
#In just one step
docker compose exec mongodb mongosh "mongodb://nombreUsuario:contraseña@localhost:27017/?authMechanism=DEFAULT&tls=false"

````sh
show dbs
show collections
`````

````sh
use ("platzi-store")

db.Productos.find()

`````

