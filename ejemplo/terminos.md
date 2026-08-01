# Página de ejemplo — no son unos términos reales

**Esto no son los términos de uso de ninguna aplicación.** Es la pareja de
[`ejemplo/privacidad`](/legal/ejemplo/privacidad), y existe por el mismo motivo.

`@nopaixxorg/legal` comprueba **los dos documentos** de cada app —privacidad y términos— con
`checkLegalUrls()`. Con solo uno publicado, cualquier app que se midiera contra `ejemplo` vería un
fallo permanente, y el ejemplo no serviría para lo que se creó.

```bash
curl -s -o /dev/null -w "%{http_code}" https://nopaixxorg.github.io/legal/ejemplo/privacidad
curl -s -o /dev/null -w "%{http_code}" https://nopaixxorg.github.io/legal/ejemplo/terminos
```

**Las dos deben devolver 200.** Si una falla, la forma de las URL ha cambiado y hay que corregirla
antes de enviar ninguna ficha a la tienda.

**No borres ninguna de las dos.** Van en pareja.

Los términos reales de cada app van en `<app>/terminos.md`.
