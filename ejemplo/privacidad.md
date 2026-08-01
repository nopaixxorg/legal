# Página de ejemplo — no es una política real

**Esto no es la política de privacidad de ninguna aplicación.** Es una página de ejemplo que
existe por dos motivos concretos:

1. **Documenta la forma de las URL** con un caso que se puede visitar:
   `https://nopaixxorg.github.io/legal/<app>/privacidad` — carpeta por app, sin extensión y
   **sin barra final**.

2. **Es la que verifica el contrato.** `@nopaixxorg/legal` compone esa URL para las 101 apps. Si
   la forma fuese distinta, las fichas de todas apuntarían a un 404 y nadie se enteraría hasta que
   un usuario lo intentara. Esta página permite comprobarlo con una orden.

```bash
curl -s -o /dev/null -w "%{http_code}" https://nopaixxorg.github.io/legal/ejemplo/privacidad
```

**No la borres.** Es barata y es lo único que mantiene esa suposición cerrada.

Las políticas reales van en `<app>/privacidad.md`, a partir de `_plantilla/privacidad.md`.
