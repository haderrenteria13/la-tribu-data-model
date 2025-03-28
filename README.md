# La Tribu - NoSQL Data Model 📚

## Descripción del Proyecto
La Tribu es una empresa de transporte de pasajeros que conecta el municipio de Bagadó, Chocó, con la ciudad de Medellín y otros destinos. Este proyecto busca diseñar una base de datos NoSQL que digitalice sus procesos, mejorando la seguridad, eficiencia y control de la información.

Link Diagrama: https://www.figma.com/design/iroarw7BrnrsuEPKglhfnC/Database-Diagram-Builder-(Community)?node-id=11-376&t=kDl1xBSzH2rCQgvw-1

![ARCHITECTURE](https://github.com/user-attachments/assets/59806980-11b6-4a3f-97b4-4946063ef3ba)

---

## Modelo de Datos
### Tipos de Datos Utilizados
- **String**: Para almacenar textos (nombres, descripciones, etc.).
- **Integer**: Para valores numéricos enteros.
- **Double**: Para valores decimales.
- **Boolean**: Para valores verdaderos o falsos.
- **Date**: Para fechas específicas.
- **Timestamp**: Para fechas con marca de tiempo precisa.
- **Array**: Para listas de elementos.
- **Object**: Para documentos embebidos.
- **ObjectID**: Identificadores únicos generados por MongoDB.

---

## Acceso a los Datos
El acceso a los datos se realizará a través de una API que facilite operaciones CRUD (Crear, Leer, Actualizar, Eliminar) para cada una de las colecciones. Se implementarán endpoints que permitan la gestión eficiente de la información.

---

## Consultas Más Comunes
- **¿Cuántos conductores hay disponibles?**
- **¿Cuántos pasajeros tiene cada viaje?**
- **¿Cuáles son los vehículos disponibles en determinado momento?**
- **¿Cuántas encomiendas se realizaron en los últimos días?**

---

## Frecuencia de Escrituras y Lecturas
- **Lecturas frecuentes:** La consulta de rutas, programación de conductores y vehículos se realizará constantemente durante el día.
- **Escrituras moderadas:** Se espera un flujo constante de creación de reservas, registros de clientes y encomiendas a medida que se gestionan los servicios.

---

## Estructura de Carpetas
```
📂 la-tribu-nosql
│
├── 📂 docs
│   ├── DATA_MODEL.md        # Explicación detallada del modelo de datos
│   └── ARCHITECTURE.jpg      # Estructura general de la aplicación
│   
│
├── 📂 data
│   ├── clientes.json
│   ├── conductores.json
│   ├── encomiendas.json
│   ├── programacion.json
│   ├── reservas.json
│   ├── roles.json
│   ├── rutas.json
│   ├── ubicacion.json
│   ├── usuarios.json
│   ├── vehiculos.json
│   └── ventas.json
│
└── README.md # Documentación general del proyecto
```
