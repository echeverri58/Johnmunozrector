# Sistema de Diseño y Documentación del Proyecto
**Campaña a la Rectoría UdeA 2026-2029 - John Mario Muñoz Lopera**

Este documento recopila todas las decisiones de diseño, la estructura del proyecto y los últimos ajustes realizados, para servir como guía y punto de restauración en futuras modificaciones.

## 1. Identidad Visual y Tema (Branding)
El sitio web está diseñado con un enfoque profesional y moderno ("Glassmorphism" y estilo minimalista) que resalta la coherencia institucional con la Universidad de Antioquia.

- **Paleta de Colores Principal:**
  - **Verde UdeA (`#0d6939`):** Usado para énfasis, bordes y acentos institucionales.
  - **Morado (`#5f57a2`):** Usado como color secundario y para efectos interactivos de *hover*.
  - **Blanco (`#ffffff`):** Usado para texto principal sobre fondos oscuros o translúcidos.
- **Tipografía:**
  - **Titulares y elementos destacados:** `Montserrat` (Pesos 800 y 900).
  - **Texto de cuerpo y navegación:** `Inter` (Pesos 300, 400 y 600).
- **Aesthetic Core:** Uso extensivo de efectos de cristal (backdrop-blur, fondos translúcidos, bordes semi-transparentes) para dar una apariencia *premium* y de alta tecnología.

## 2. Tecnologías y Estructura
- **Framework de Estilos:** Tailwind CSS integrado vía CDN (Configurado dinámicamente en el `<head>` del HTML).
- **Íconos:** Material Icons de Google.
- **Estructura del Proyecto:** Todo el código final y funcional se encuentra en las carpetas `diseño 5` y `diseño 6`.

## 3. Elementos Clave y Ajustes Finales

### Cabecera y Hero Section (Inicio)
- Se actualizó el slogan principal a: **"Conocimiento, coherencia y experiencia para liderar el futuro de la UdeA."**
- Los botones de acciones secundarias ("Plan rectoral", "Conoce más") fueron removidos del *Hero* para mantener la interfaz lo más limpia posible, redirigiendo la atención a la navegación principal.

### Imágenes y Recursos Gráficos
- **Logos:** Los logos principales de la cabecera (`logo_nav.png`) y el pie de página (`logo_footer.png`) se sirven de manera local para asegurar su correcta carga tras el despliegue.
- **Favicon:** Se integró la imagen personalizada `logofavicon.png` (renombrada a `favicon.png`) para que aparezca en las pestañas de los navegadores.
- **Sección Trayectoria:** Se utiliza la imagen `portada_trayectoria.jpeg`. Se retiró un desvanecido verde que tenía previamente y se le aplicó un resplandor luminoso blanco (*hover glow*) que reacciona de manera dinámica al paso del cursor.

### Enlaces y Contacto
- Todos los botones que tienen el ícono de arroba (`@`), así como las menciones de correo electrónico a lo largo de la página (tanto en el pie de página como en la sección de Contacto), fueron unificados para dirigir hacia el correo institucional: **`john.munoz@udea.edu.co`** en lugar de correos genéricos anteriores.

## 4. Flujo de Publicación (Hosting & GitHub)
- **Repositorio Activo:** [https://github.com/echeverri58/Johnmunozrector.git](https://github.com/echeverri58/Johnmunozrector.git)
- **Zip para Hosting Privado:** Se generó el paquete `Landing_Page_John_Mario_UdeA.zip` dentro de la carpeta `diseño 6` que encapsula todos los archivos (HTML e imágenes enlazadas) listos para subirse a cualquier servicio de Hosting externo.
- **Rutas y Referencias:** Se corrigieron y garantizaron todas las referencias a los archivos para que sean de carácter relativo (e.g., `src="logo_nav.png"`), evitando así errores de origen cruzado (`404 Not Found`) cuando se publican los sitios tanto en GitHub Pages como en plataformas de terceros.

---
> **Nota de restauración:** Si se requiere deshacer cambios futuros o recuperar la versión más estable lograda, asegúrate de mantener intacta la estructura interna de las carpetas `diseño 5` y `diseño 6` tal cual como fueron empaquetadas en el archivo `.zip`.
