# Hola Mundo — Academia de español online para niños y adolescentes

Sitio web de **Hola Mundo**, academia de español online y en vivo para estudiantes de 8 a 17 años, operada por **Educamax Ltda** (RUT 77.912.943-8), Chile.

**Sitio publicado:** https://holamundoacademy.com/
**Versión en español:** https://holamundoacademy.com/?lang=es

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | Todo el sitio: contenido, estilos y código en un solo archivo |
| `og-image.jpg` | Imagen que aparece al compartir el enlace en redes y WhatsApp (1200×630) |
| `sitemap.xml` | Le indica a Google las versiones en inglés y español |
| `hola_mundo_*.png` | Ilustraciones originales (la de portada es la base de `og-image.jpg`) |

## Cómo editar lo más común

Todo está dentro de `index.html`, en la parte de `<script>` al final del archivo.

- **Datos de la empresa y del formulario:** objeto `HOLA_CONFIG` (correo de contacto, `FORM_ENDPOINT`, `LEGAL_ENTITY`).
- **Textos en inglés y español:** objeto `HOLA_I18N.translations`, con una sección `en` y otra `es`. Cada texto tiene la misma clave en ambos idiomas (por ejemplo `price_title`). Si cambias uno, cambia también el otro.
- **Precio:** claves `price_*` en las traducciones, el número `100` en la sección `id="pricing"`, la pregunta frecuente `faq-9` y el bloque `"offers"` de los datos estructurados (`application/ld+json`, al inicio del archivo).
- **Preguntas frecuentes, programas y misiones:** objeto `HOLA_DATA`.
- **Política de privacidad:** función `privacyPolicyHTML` (versión en español e inglés). Al modificarla, actualiza `policyVersion` y `policyUpdated` en `LEGAL_ENTITY`.

## Formulario de clase de prueba

Las solicitudes se envían con [FormSubmit](https://formsubmit.co/) a `educamaxcl@gmail.com`. El formulario ya está activado y funciona desde `holamundoacademy.com`. Si se cambia el correo de destino, FormSubmit pedirá confirmarlo de nuevo por correo.

## Publicar cambios

El sitio se publica automáticamente en **Vercel** (dominio `holamundoacademy.com`) cada vez que se suben cambios a la rama `main`. Después de editar:

```
git add .
git commit -m "Describe el cambio"
git push
```

El sitio se actualiza en 1–2 minutos.

## Pendientes

- Revisión legal de la política de privacidad (Ley 21.719, vigente desde el 1 de diciembre de 2026).
- Horarios y tamaño máximo de los grupos.
- Fotos propias en lugar de las de Unsplash, y profesores con nombre y foto.
- Registrar `holamundoacademy.com` en Google Search Console y enviar `https://holamundoacademy.com/sitemap.xml`.
