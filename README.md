# El repositorio de Código Fuente

## Estructura de Carpetas

recomendamos una estructura de carpetas como se detalle a continuación

```
.
├── docs                    # Archivos de documentacion
├── src                     # Código fuente
├── tests                   # Codigo de Pruebas 
├── tools                   # herramientas y utilidades que se necesiten
├── LICENSE
├── .gitignore              # archivo con los filtros para los archivos que se deben versionar.
└── README.md

```

## El archivo README

Es la documento que debe dar una descripción del proyecto/producto que es versionado en el repositorio actual. Recomendamos usar el siguiente [template](http://bit.ly/readme-md) para detallar el contenido.


## Documentación

La documentación de un proyecto se compone:
- Codigo Fuente (principalmente)
- Especificaciones: Historias de Usuario + Criterios de Aceptación + Escenarios que validan los Criterios de aceptación.
- Los reportes de ejecucion de las pruebas: Unitarias, Funcionales, Integración, Seguridad, Performance, etc.
- La documentación técnica que se necesite y sea valiosa como: Diagramas de diseño, despliegue, secuencia, etc. Para éste componente de la documentación recomendamos usar la siguiente estructura.

```
.
├── ...
├── docs                    # Archivos de documentacion
│   ├── TOC.md              # Tabla de contenido
│   ├── faq.md              # Preguntas frecuentes
│   ├── misc.md             # Informacion adicional
│   ├── usage.md            # Uso de la documentación
│   ├── Features            # Folder para las caracteristicas del producto que necesitan documentación
│   └── ...                 # etc.
└── ...

```

## Código de Pruebas

El codigo de pruebas es importante, y debería mantenerse en el mismo repositorio de esta forma los cambios en el codigo fuente implican: cambios en el codigo de produccion y codigo de pruebas.

```
.
├── ...
├── test                    
│   ├── benchmarks          # pruebas de estress y carga
│   ├── integration         # pruebas de integración de servicios
│   ├── e2e                 # pruebas de aceptación de usuario o funcionales
│   └── unit                # Pruebas unitarias
└── ...

```

## Codigo fuente (codigo de producción)

Es el código que se despliega en producción y que da vida a la solución. Aqui depende de las herramientas, lenguajes, paradigmas a utilizar. 

Organizar el codigo fuente caracteristicas / componentes / paginas y/o clases no roles.

Todo esto debajo de la carpeta "src".
```
.
...
├── preferences
|   ├── PreferencesController.java
|   ├── NewPreference.java
|   ├── CreatePreferenceHandler.js
|   └── CreatePreference.js
├── authentication
|   ├── AuthenticationController.java
|   ├── LoginAttempt.java
|   ├── LoginAttemptHandler.java
|   └── InvalidCredentialsException.java
...

```

## Herramientas 

Aqui se guardan aquellas herramientas que no se puedan descargar usando algun manejador de paquetes como npm, mvn, nuget, gradle, etc.
