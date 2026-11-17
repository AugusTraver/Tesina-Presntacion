# Cómo controlar una IA que nos supere · presentación

Presentación inmersiva en 3D de la tesina de Augusto Traverso (5° E · TEI 2026). Es un solo `index.html`, sin compilación, hecho con three.js y GSAP.

- `index.html`: la presentación.
- `GUION.md`: guion por diapositiva, con tiempos, acciones y preguntas probables.

## Abrirla

Abrí `index.html` en **Chrome o Edge, con internet**: las librerías y las fuentes se cargan desde la web. No funciona en la vista previa de VS Code.

## Publicarla

- **Netlify Drop:** arrastrá la carpeta a https://app.netlify.com/drop.
- **Vercel:** importá el repositorio, elegí el preset *Other* y dejá vacío el comando de build.
- **GitHub Pages:** Settings → Pages → *Deploy from a branch* y elegí la rama.

## Controles

| Tecla | Acción |
|---|---|
| `→` `espacio` | siguiente (avanza los pasos internos) |
| `←` | anterior |
| `1`–`9`, `0` | saltar a la diapositiva 1–10 |
| `N` | notas del orador |
| `F` | pantalla completa |
| swipe | navegar en el celular |

En la diapositiva 2 hay un botón *Aprobar* que se puede tocar. En la 3 hay dos controles deslizantes para la simulación ilustrativa. Las diapositivas 6, 7, 8 y 10 tienen pasos internos.

## Pendiente de revisar

- El link del episodio de 80,000 Hours (diapositiva 9) apunta a `80000hours.org/podcast/episodes/buck-shlegeris-ai-control-scheming/`. No se pudo verificar desde el entorno donde se armó: comprobalo y, si querés, reemplazalo por el video de YouTube con `&t=1998s` (33:18).
