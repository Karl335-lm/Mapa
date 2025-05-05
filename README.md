# Mapa
Esta es una aplicación de escritorio en Java que permite visualizar mapas, buscar lugares, cambiar el tipo de mapa (carretera, satélite, híbrido, terreno) y controlar el nivel de zoom. Utiliza `JXMapViewer2` y la API de OpenStreetMap (Nominatim) para realizar búsquedas geográficas.
## 📋 Características

- 🧭 Búsqueda de lugares por nombre o dirección.
- 🔍 Control de zoom (acercar y alejar).
- 🗺️ Cambio de tipo de mapa (roadmap, satélite, híbrido, terreno).
- 📍 Marcador de ubicación en los resultados de búsqueda.

---

## 🧱 Componentes

### `PruebaMapa.java`
- Ventana principal (`JFrame`) que contiene:
  - Campo de texto para búsqueda.
  - Botones para buscar, acercar y alejar el zoom.
  - ComboBox para seleccionar el tipo de mapa.
  - El panel `mapss` que muestra el mapa.
[![Captura-de-pantalla-2025-05-04-230806.png](https://i.postimg.cc/66fP7jX7/Captura-de-pantalla-2025-05-04-230806.png)](https://postimg.cc/z3376k35)
### `mapss.java`
- Panel personalizado (`JPanel`) que incluye:
  - `JXMapViewer` como visor del mapa.
  - Métodos para:
    - Buscar lugares usando OpenStreetMap.
    - Cambiar el tipo de mapa.
    - Pintar marcadores en el mapa.
      [![Captura-de-pantalla-2025-05-04-222729.png](https://i.postimg.cc/k5L0cB1B/Captura-de-pantalla-2025-05-04-222729.png)](https://postimg.cc/d7mNQtKY)
## ▶️ Instrucciones de uso

1. **Requisitos:**
   - JDK 8 o superior.
   - Conexión a Internet.
2. **Ejecutar:**
   - Ejecuta `PruebaMapa.java`.
   - Escribe una dirección o nombre de lugar en el campo de texto.
   - Haz clic en "Buscar" para centrar el mapa en ese lugar.
   - Usa "Maximizar" o "Minimizar" para ajustar el zoom.
   - Cambia el tipo de mapa con el menú desplegable.
[![Captura-de-pantalla-2025-05-04-230915.png](https://i.postimg.cc/8Pk0LRpZ/Captura-de-pantalla-2025-05-04-230915.png)](https://postimg.cc/F1qp4JJS)
---

## ⚙️ Dependencias

Asegúrate de incluir las siguientes librerías:
- CONEXIÓN A INTERNET
- [`jxmapviewer2`]
- [`org.json`]
  [![Captura-de-pantalla-2025-05-04-231045.png](https://i.postimg.cc/25WcCTGS/Captura-de-pantalla-2025-05-04-231045.png)](https://postimg.cc/Ff9gZywM)
  
##Métodos y proiedades relevantes
Método                              / Propiedad	              Clase	Descripción

buscarLugar(String nombreLugar)	            mapss      Realiza una búsqueda con Nominatim (OpenStreetMap) y posiciona el mapa.

setTileFactory(TileFactory factory)         mapss	     Cambia el tipo de mapa (carretera, satélite, híbrido, terreno).

getMapViewer()	                            mapss	     Retorna la instancia de JXMapViewer.

btnBuscarActionPerformed(evt)          	PruebaMapa	   Toma el texto del campo y llama a buscarLugar().

btnMinimizarActionPerformed(evt)	      PruebaMapa    	Aumenta el zoom del mapa.

btnMaximizarActionPerformed(evt)	      PruebaMapa	    Reduce el zoom del mapa.

CambioMapaActionPerformed(evt)	    PruebaMapa	Cambia el tipo de mapa según selección del usuario.

##Link de Youtube
https://www.youtube.com/watch?v=hWe15AjwnNk

##Javadoc
[javadoc.zip](https://github.com/user-attachments/files/20031937/javadoc.zip)


