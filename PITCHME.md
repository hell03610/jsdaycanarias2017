# Me casé con <span class="gold">EmberJS</span>
#### y no vas a creer que pasó a continuación

---

## Conociendo al novio: EmberJS en un pispás

 - Aquí quien manda es la url
 - Página = Route + template
 - Y quien sirve los datos?
 - Componentes, componentes *everywhere*

---

## ¿Cómo es estar casad@ con EmberJS?

---

Te permite estar <span class="gold">enfocad@ en desarrollar</span> y publicar nuevas características en tu producto.

Para ello te brinda un rico ecosistema de ** tooling, testing, addons y ayuda**

---

### Tooling

 1. ember-cli
 2. inspector de navegador
 3. twiddle

---

###### ember-cli

```
 npm install -g ember-cli 
```

Utilidad de linea de comandos basada en Broccoli, babel, ~npm y bower~, yarn

---

###### ember-cli

```shell
> ember new jsday
```

@[1](Crea nuevos proyectos sin preocuparte de su estructura)

--- 

###### ember-cli

```shell
|-app
|-config
|-node_modules
|-public
|-tests
|-vendor
ember-cli-build.js
package.json
README.md
testem.js
```

@[1](La mayor parte del código caerá aquí: modelos, rutas, componentes...)
@[2](Configuración del proyecto: rutas base para apis, flags, etc)
@[4](Carpeta para assets públicos: imagenes y fuentes)
@[5](Tests para los modelos, rutas, componentes...)
@[6](Carpeta para librerías de terceros no gestionadas)
@[7](Configura como se construye el proyecto)

---

###### ember-cli

```shell
> ember generate route contact-us

installing route
  create app/contact-us/route.js
  create app/contact-us/template.hbs
updating router
  add route contact-us
installing route-test
  create tests/unit/contact-us/route-test.js
```

<span class="aside">Generadores: usa los generadores _built-in_ para seguir las prácticas más actuales (y sus correspondientes tests) </span>

---

###### ember-cli

```shell
> ember serve
> ember build
> ember build --environment="production"
```

@[1](Sirve el proyecto con un servidor de desarrollo)
@[2](Construye el proyecto para desarrollo, por defecto en "dist/")
@[3](Construye el proyecto para producción, por defecto en "dist/")

<span class="aside">Construcción del proyecto: compilación de assets, finger-printing y gestión del pipeline de deploy</span>

---

###### ember-cli

```shell
> ember build --environment="production"

cleaning up...
Built project successfully. Stored in "dist/".
File sizes:
 - dist/assets/jsday-af67185be14051fe394486ee1961dbaf.js: 5.38 KB (1.39 KB gzipped)
 - dist/assets/jsday-d41d8cd98f00b204e9800998ecf8427e.css: 0 B
 - dist/assets/vendor-d41d8cd98f00b204e9800998ecf8427e.css: 0 B
 - dist/assets/vendor-fd395a08caa91c093a31c61257b69910.js: 737.24 KB (191.02 KB gzipped)
```

---

### Testing

 - Totalmente integrado en el framework
 - Explicado en la web
 - 3 niveles: unitario, integración, aceptación

---

### Addons
 - Expande las capacidades basicas de EmberJS
 - EmberData
 - Mantenidos por la comunidad, alguno de los mas importantes

+++

### Ayuda

 - Tutorial en la web
 - Slack
 - Otros recursos

---

## ¿Qué hay de nuevo, viejo?

+++

### Actualizando el framework
 
 - Release cicle, canary
 - LTS 
 - Deprecations
 - Blog post
 - RFC

### Y qué hubo de nuevo?

 - GlimmerJS

### Que se cuece en el horno
 
 - boardstatus
 - glimmer -> components

---

## Consejos matrimoniales

Consejos para elegir un framework sobre el que construir tu producto

 - Voy a tener que añadir funcionalidad a un ritmo sostenible, como de bien esta orientado a test?
 - Puede que mi equipo crezca, que documentacion y guias hay? 
 - Cuanta burocracia conlleva? Tiene ya integrado tooling para deploy pipelines, test runners, gestion del estado, builds de desarrollo y produccion, asset figerprinting and cache busting?
 - Voy a tener que mantener este producto durante un tiempo, que release plan tiene? Como de facil o doloroso es actualizar versiones? Tiene LTS?
 - Quien mantiene el framework? Como evoluciona? Hay alguna compañia detras o es mantenido por una comunidad?

---

## Dos no se pelean si uno no quiere

 - Por mucho que escogas el framework *perfecto* tambien tienes que poner de tu parte para que el proyecto no se te vaya de las manos

 - Good design
 - Simple responsability
 - Good naming
 - Tested

 - Extra ball: UI guide based on components

---

## Q & A
