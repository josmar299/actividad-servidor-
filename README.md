# Reporte de Desarrollo
la conexión con Meilisearch

La conexión con Meilisearch se realiza utilizando la biblioteca oficial de JavaScript de Meilisearch. y Meilisearch es mu motor de busqueda en el cual se puede buscar cual quier pelicula 
```javascript
const client = new MeiliSearch({
  host: 'http://172.233.139.197',
  apiKey: 'd388d2446bccc07114debedcca01058d239ee3afd4553c93c6f1ad7bea61',
});
```
 el índice de películas llamado  peliculas , se utiliza el método search() del cliente. Este método toma como parámetro la consulta ingresada por el usuario y devuelve los resultados coincidentes en el índice especificado y no se muestra nada es que la busqueda no fue encontrada 
 

# Realización de la búsqueda:
Al hacer clic en el botón "Buscar", se ejecuta la función manejar Busqueda, que realiza la consulta al índice de Meilisearch.
Los resultados se actualizan en el estado resultados y se muestran en la interfaz de usuario.

Personalizaciones implementadas en la aplicaciónsensibilidad al brillo.
Se implementó un diseño adaptable para la lista de resultados, usando flexbox para permitir una distribución uniforme y atractiva de los elementos.
## Mensajes de error:
aqui cuando no se encuentra ninguna busqueda de  pelicula 
## Valores predeterminados:
En caso de que los datos de una película no incluyan un póster o un título, se proporcionan valores predeterminados como una imagen genérica y el texto “Sin título”.
