# legal — Políticas y términos de las apps de 101apps

Este repositorio aloja las **políticas de privacidad** y los **términos de uso** de las
aplicaciones del reto **101apps**, publicados con GitHub Pages.

```
https://nopaixxorg.github.io/legal/<app>/privacidad
https://nopaixxorg.github.io/legal/<app>/terminos
```

---

## Por qué este repositorio es público — no lo cambies

**Es la única excepción a que todo el proyecto sea privado (hq/DECISIONES.md, D-005), y es
deliberada.**

Una política de privacidad **tiene que ser accesible sin autenticación**: Google Play exige una
URL pública y la comprueba. Si este repositorio pasara a privado, **todas las URL devolverían 404
y las fichas de las 101 apps quedarían incumpliendo**, sin que nada avisara.

Es exactamente el tipo de «arreglo» bienintencionado del que advierte `hq`: hacerlo privado
parecería coherente con el resto del proyecto y rompería la publicación entera.

**Aquí no va nada que no deba ser público.** Ni claves, ni datos personales, ni configuración.

---

## Estructura

```
index.md              Índice público de apps
<app>/privacidad.md   Política de privacidad de esa app
<app>/terminos.md     Términos de uso de esa app
_plantilla/           Plantillas. Jekyll NO publica lo que empieza por «_»
```

---

## Al dar de alta una app

1. Copiar `_plantilla/privacidad.md` a `<app>/privacidad.md` y rellenar los campos marcados.
2. Añadir la app a `index.md`.
3. Comprobar que la URL responde **200 antes** de enviar la ficha a Google.

Ese último paso no es burocracia: es la comprobación por efecto que exige `hq` (D-028). Que el
fichero esté en el repositorio no demuestra que la URL funcione.

---

## Pendiente

- **Propietario definitivo:** el futuro `role-legal` (D-019 previsto en `hq/INDICE.md`).
  Mientras no exista, lo mantiene `hq`.
- **Los textos de la plantilla no están revisados por nadie con criterio legal.** Ver el aviso
  dentro de `_plantilla/`.
