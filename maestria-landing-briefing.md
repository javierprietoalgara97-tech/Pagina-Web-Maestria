# MaestrIA — Briefing Landing Page

---

## 1. Información general del proyecto

| Campo | Detalle |
|---|---|
| **Nombre de la marca** | MaestrIA |
| **Tipo de web** | Landing page (una sola página) |
| **Idioma** | Español |
| **Tecnología de despliegue** | GitHub + Vercel |
| **Construcción** | Manual desde editor / Claude |

---

## 2. Identidad de marca

### Colores corporativos

| Color | Uso |
|---|---|
| `#F5C518` — Amarillo MaestrIA | Acentos, CTAs primarios, números destacados |
| `#0B0B0F` — Negro profundo | Fondo principal, texto sobre fondos claros |
| `#3A3A3A` — Gris mate | Fondos secundarios, tarjetas, bordes sutiles |
| `#FFFFFF` — Blanco | Texto principal sobre fondo oscuro |
| `rgba(255,255,255,0.72)` — Blanco suave | Texto secundario, subtítulos, cuerpos de texto |

### Tipografía
- **Estilo:** Moderna, sans-serif, peso 800 para titulares
- **Tono visual:** Oscuro con acentos en amarillo dorado — denso, profesional, cercano

### Logo
- Archivo: colocar en `/assets/logo-maestria.svg` (o `.png`)
- Ubicación en la web: esquina superior izquierda del header/nav

### Tono de comunicación
- Cercano pero profesional
- Directo, sin tecnicismos innecesarios
- Orientado al beneficio del cliente, no a la tecnología por sí misma

---

## 3. Público objetivo

- **Perfil:** Dueños de PYME y directivos
- **Sector:** Empresas con departamento de atención al cliente y/o ventas
- **Pain points:**
  - Equipos desbordados atendiendo tareas repetitivas
  - Dificultad para escalar sin aumentar plantilla
  - Leads que no se reactivan, pipeline de ventas desorganizado

---

## 4. Servicios ofrecidos

MaestrIA se especializa en soluciones de IA para los departamentos de **atención al cliente y ventas**. No es consultoría generalista: es especialización funcional.

| Servicio | Descripción breve |
|---|---|
| **Agentes de WhatsApp** | Automatización de conversaciones y atención 24/7 vía WhatsApp |
| **Agentes para RRSS** | Gestión y respuesta automatizada en redes sociales |
| **CRM con IA** | CRM inteligente con automatizaciones para seguimiento de clientes |
| **Plataforma de reactivación de leads** | Sistema para recuperar clientes inactivos o leads fríos |
| **Soluciones personalizadas** | Desarrollo a medida según las necesidades del negocio |

---

## 5. Propuesta de valor

> Ayudo a negocios a implementar la IA en la parte de soporte y ventas para ahorrarse entre 10 y 15 horas semanales, para que puedan escalar el negocio y mejorar la eficiencia operativa.

---

## 6. Estructura de la landing (secciones en orden)

### SECCIÓN 01 — Hero

**Referencia visual:** `01-hero.html`
**Componentes a replicar:**
- Layout grid 2 columnas: copy izquierda / elemento visual derecha (foto o ilustración)
- Fondo oscuro `#0B0B0F`
- Eyebrow text en mayúsculas y tracking amplio (color `rgba(255,255,255,0.60)`)
- H1 tipografía grande, peso 800, `clamp(38px, 5.5vw, 68px)`
- Subtítulo y cuerpo en blanco suave
- Dos CTAs apilados (ver sección 8)
- Animación reveal: slide desde la izquierda con IntersectionObserver

**Texto:**
```
EYEBROW: CONSULTORÍA DE IA · MAESTRIA

H1: Automatizo procesos en el departamento de atención al cliente y ventas para que los negocios puedan escalar y mejorar la eficiencia.

SUBTÍTULO: Para que puedan centrarse en las tareas que realmente importan y atender cada vez a más clientes.
```

---

### SECCIÓN 02 — Propuesta de valor

**Referencia visual:** `04-refinamientos.html` (banda de impacto)
**Componentes a replicar:**
- Banda corta centrada, fondo contrastado `#0B0B0F` con borde `rgba(245,197,24,0.22)` (amarillo MaestrIA)
- Tipografía grande, peso 800
- Color del texto principal: `#F5C518` (amarillo MaestrIA en lugar de `#e9dcc7`)
- Texto en itálica de cierre en blanco
- Animación: fade desde abajo con IntersectionObserver

**Texto:**
```
H2: Ayudo a negocios a implementar la IA en la parte de soporte y ventas para ahorrarse entre 10 y 15 horas semanales.

CUERPO: Para que puedan escalar el negocio y mejorar la eficiencia operativa.
```

---

### SECCIÓN 03 — ¿Qué puedo hacer por tu negocio?

**Referencia visual:** `02-esto-no-es-un-curso.html` (dos columnas de bullets)
**Componentes a replicar:**
- Titular + intro en prosa
- Dos columnas de cards con glassmorphism (`rgba(255,255,255,0.07)`, `backdrop-filter: blur`)
- Borde sutil `rgba(255,255,255,0.14)`
- Label de columna en mayúsculas y amarillo MaestrIA
- Items con flecha `→` en amarillo MaestrIA
- Animación: slide izquierda/derecha alternado

**Texto:**
```
H2: ¿Qué puedo hacer por tu negocio?

INTRO: Trabajo con negocios que quieren dejar de perder tiempo en tareas repetitivas y empezar a crecer de forma inteligente. Estas son las áreas donde actúo.

COLUMNA IZQUIERDA — ATENCIÓN AL CLIENTE:
→ Agentes de WhatsApp para atención 24/7
→ Agentes para RRSS
→ Reducción de tiempos de respuesta y carga de trabajo del equipo

COLUMNA DERECHA — VENTAS Y CRM:
→ CRM inteligente con automatizaciones
→ Plataforma de reactivación de leads
→ Soluciones personalizadas a medida
```

---

### SECCIÓN 04 — Servicios (tarjetas detalladas)

**Referencia visual:** `05-que-aprenderas.html` (grid 2×2 numerado)
**Componentes a replicar:**
- Grid 2×2 en escritorio, apilado en móvil
- Cada tarjeta: número circular fondo amarillo MaestrIA / texto negro, título, descripción
- Glassmorphism en cada card
- Hover: borde amarillo suave + sombra ampliada
- Animación: alternado izquierda/derecha por columna

**Contenido de las 5 tarjetas** (la quinta puede ocupar el ancho completo o centrarse):

| # | Título | Descripción |
|---|---|---|
| 1 | Agentes de WhatsApp | Automatiza la atención al cliente en WhatsApp con agentes de IA que responden, cualifican y derivan consultas las 24 horas, sin intervención humana. |
| 2 | Agentes para RRSS | Gestiona y responde de forma automática los mensajes e interacciones en redes sociales, manteniendo la consistencia de marca y reduciendo el tiempo de respuesta. |
| 3 | CRM con IA | Un CRM inteligente que automatiza el seguimiento de clientes, prioriza oportunidades y elimina las tareas manuales del equipo de ventas. |
| 4 | Plataforma de reactivación de leads | Recupera clientes inactivos y leads fríos con secuencias automatizadas y personalizadas que vuelven a generar interés sin esfuerzo manual. |
| 5 | Soluciones personalizadas | Si tu negocio tiene necesidades específicas, desarrollo soluciones a medida que se integran con tus herramientas actuales. |

---

### SECCIÓN 05 — ¿Es para ti?

**Referencia visual:** `06-es-para-ti.html` (dos columnas sí/no)
**Componentes a replicar:**
- Dos columnas paralelas: verde (sí) / gris neutro (no)
- Badge circular ✓ / ✕
- Glassmorphism
- Animación: izquierda desde izquierda, derecha desde derecha

**Texto:**
```
COLUMNA SÍ:
✓ Tienes un equipo que pierde tiempo respondiendo siempre las mismas preguntas.
✓ Quieres escalar tu negocio sin contratar más personal.
✓ Tienes leads que no se están trabajando bien.
✓ Quieres mejorar la experiencia de tus clientes sin aumentar costes.

COLUMNA NO:
✕ Buscas una solución mágica que funcione sola sin ningún proceso previo.
✕ No estás dispuesto a adaptar mínimamente tus flujos de trabajo.
✕ Necesitas resultados sin ninguna implementación.
```

---

### SECCIÓN 06 — Testimonios

**Referencia visual:** `10-testimonios.html` (destacado + carrusel)
**Componentes a replicar:**
- Titular con efecto de anillo animado SVG
- Tarjeta destacada fondo amarillo MaestrIA (`#F5C518`), texto negro
- Carrusel de tarjetas secundarias con glassmorphism
- Botones de navegación ‹ › con animación de pulso
- Dots indicadores
- Swipe táctil habilitado

**⚠️ Estado actual:** Sin testimonios reales. Opciones:
- **Opción A (recomendada):** Sección oculta hasta tener 2-3 testimonios reales. Activar cuando estén disponibles.
- **Opción B:** Mostrar la estructura con placeholder visual: `"Tu testimonio aquí — próximamente"` sin nombres ni empresas ficticias.

---

### SECCIÓN 07 — Sobre mí

**Referencia visual:** `08-quien-imparte.html` (bloque principal con foto + copy)
**Componentes a replicar:**
- Grid: foto izquierda (con efecto flip card opcional) / texto derecha
- Tag en mayúsculas y amarillo MaestrIA: "CONSULTOR DE IA"
- Nombre en tipografía grande peso 800
- Bio en párrafos con `color: rgba(255,255,255,0.80)`
- Animación: reveal desde abajo

**Foto:** `[PENDIENTE — añadir ruta de imagen: /assets/foto-javier-prieto.jpg]`

**Texto (tal como lo proporcionó el cliente):**
```
TAG: CONSULTOR DE IA · ESPECIALISTA EN MARKETING DIGITAL

NOMBRE: Javier Prieto

BIO:
Mi nombre es Javier Prieto, soy consultor de IA profesional y especialista en marketing digital. Trabajo en empresas como especialista en estrategia digital y Estrategia de IA. Me gusta tener un trato cercano con mis clientes e implicarme al máximo en cada proyecto que desarrollo.

Me encanta hablar sobre inteligencia artificial y la parte de formar a mis clientes para que puedan sacarle el máximo partido a las soluciones que desarrollo.

Empecé como estratega en marketing digital, hasta que descubrí el mundo de la inteligencia artificial y las automatizaciones y decidí especializarme en esta área porque me apasiona.
```

> **Nota:** Se han corregido únicamente las erratas tipográficas del texto original ("Automatizao" → "Automatizo", "solcuiones" → "soluciones", "decidi" → "decidí", etc.) manteniendo íntegramente el mensaje y el tono del cliente.

---

### SECCIÓN 08 — FAQ

**Referencia visual:** `13-faq.html` (acordeón)
**Componentes a replicar:**
- Acordeón: clic en pregunta → expande respuesta con animación `max-height`
- Borde exterior `rgba(255,255,255,0.12)`, `border-radius: 20px`
- Fondo de pregunta activa con tinte amarillo MaestrIA
- Icono `+` que rota a `×` al expandir
- Animación reveal: slide desde izquierda

**Preguntas sugeridas** *(pendiente de revisión y aprobación por el cliente):*

```
P1: ¿Cuánto tiempo tarda la implementación?
R: Depende de la solución, pero la mayoría de implementaciones estándar están listas en 2 a 4 semanas. Las soluciones personalizadas pueden requerir algo más de tiempo según la complejidad.

P2: ¿Necesito conocimientos técnicos para usar las soluciones?
R: No. Diseño todas las soluciones para que sean fáciles de usar desde el primer día. Además, formo a tu equipo para que pueda sacarles el máximo partido sin depender de mí.

P3: ¿Con qué herramientas y CRMs trabajas?
R: Trabajo con las principales plataformas del mercado. Antes de empezar cualquier proyecto analizamos tus herramientas actuales para asegurar la integración.

P4: ¿Qué pasa si la solución no funciona como esperaba?
R: Me implico al máximo en cada proyecto. Si algo no funciona como debe, lo ajustamos. Mi objetivo es que veas resultados reales, no solo entregar una solución.

P5: ¿Cuánto cuesta contratar tus servicios?
R: Cada proyecto es diferente, por eso ofrezco una llamada gratuita de diagnóstico antes de hablar de precios. Así puedo darte una propuesta ajustada a tu caso concreto.
```

---

### SECCIÓN 09 — CTA Final

**Referencia visual:** `11-inscripcion-precio.html` (zona de CTA/precio) — adaptado a una sola tarjeta de contacto
**Componentes a replicar:**
- Banda o tarjeta centrada de alto impacto
- Fondo: `#F5C518` (amarillo MaestrIA), texto negro
- Titular grande en peso 800
- CTA botón oscuro con hover

**Texto:**
```
H2: ¿Listo para automatizar y escalar tu negocio?

CUERPO: Reserva una llamada gratuita y analizamos juntos qué soluciones pueden funcionar mejor para tu empresa.

BOTÓN CTA: Reservar llamada gratuita
```

---

## 7. Call to Action principal

- **Plataforma:** Cal.com
- **Enlace:** `[PENDIENTE — añadir enlace de Cal.com]`
- **Texto del botón:** "Reservar llamada gratuita"
- **Comportamiento:** Abrir en nueva pestaña (`target="_blank"`)

---

## 8. Navegación / Header

- Logo MaestrIA (izquierda)
- Links de navegación: Servicios · Sobre mí · FAQ · Contacto
- CTA fijo en header: "Reservar llamada" (botón amarillo pequeño)
- Comportamiento scroll: header con `backdrop-filter: blur` al hacer scroll

---

## 9. Footer

- Logo pequeño
- Links legales: Política de privacidad · Aviso legal *(pendiente de redactar)*
- Email de contacto: `[PENDIENTE]`
- Redes sociales: `[PENDIENTE — añadir perfiles]`
- Texto copyright: `© 2025 MaestrIA · Javier Prieto`

---

## 10. Elementos visuales y componentes reutilizables del código de referencia

Estos componentes están documentados en el código fuente adjunto y deben adaptarse con los colores de MaestrIA:

| Componente | Archivo origen | Cambio de color principal |
|---|---|---|
| Hero reveal (slide izq.) | `01-hero.html` | Sin cambio de estructura |
| Banda de impacto | `04-refinamientos.html` | `#e9dcc7` → `#F5C518` |
| Cards con glassmorphism | `05-que-aprenderas.html` | Números: fondo `#F5C518`, texto `#0B0B0F` |
| Dos columnas sí/no | `06-es-para-ti.html` | Sin cambio de estructura |
| Timeline vertical | `07-tu-dia.html` | Puntos y horas: `#e9dcc7` → `#F5C518` |
| Flip card foto + bio | `08-quien-imparte.html` | Tag color: `#F5C518` |
| Carrusel de imágenes | `09-galeria.html` | Sin cambio de estructura |
| Testimonios + carrusel | `10-testimonios.html` | Tarjeta destacada: fondo `#F5C518`, texto `#0B0B0F` |
| Acordeón FAQ | `13-faq.html` | Pregunta activa: tinte `rgba(245,197,24,0.08)` |
| IntersectionObserver reveal | Todos los archivos | Patrón reutilizable en cada sección |

### Patrón de animación reveal (estándar MaestrIA)
```javascript
// Reutilizar en cada sección con prefijo de clase único
const io = new IntersectionObserver((entries, obs) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('mae-visible');
      obs.unobserve(entry.target);
    }
  });
}, { threshold: 0.18, rootMargin: '0px 0px -6% 0px' });
```

### Variables CSS globales MaestrIA
```css
:root {
  --mae-amarillo: #F5C518;
  --mae-negro: #0B0B0F;
  --mae-gris: #3A3A3A;
  --mae-blanco: #FFFFFF;
  --mae-blanco-suave: rgba(255, 255, 255, 0.72);
  --mae-glass-bg: rgba(255, 255, 255, 0.07);
  --mae-glass-border: rgba(255, 255, 255, 0.14);
  --mae-amarillo-tinte: rgba(245, 197, 24, 0.10);
  --mae-amarillo-border: rgba(245, 197, 24, 0.28);
  --mae-radio: 22px;
  --mae-shadow: 0 20px 50px rgba(0, 0, 0, 0.25);
}
```

---

## 11. Assets pendientes de añadir

| Asset | Estado | Ruta destino |
|---|---|---|
| Logo MaestrIA | Pendiente | `/assets/logo-maestria.svg` |
| Foto Javier Prieto | Pendiente (cliente lo añadirá) | `/assets/foto-javier-prieto.jpg` |
| Enlace Cal.com | Pendiente | Secciones Hero y CTA Final |
| Email de contacto | Pendiente | Footer |
| Perfiles RRSS | Pendiente | Footer |
| Textos legales | Pendiente | Footer |

---

## 12. Estructura de archivos del proyecto

```
maestria-landing/
├── index.html              ← Landing principal
├── assets/
│   ├── logo-maestria.svg
│   └── foto-javier-prieto.jpg
├── css/
│   └── styles.css          ← Variables globales + reset + layout base
├── js/
│   └── main.js             ← IntersectionObserver + acordeón + carrusel
└── README.md               ← Este archivo
```

---

*Documento de briefing generado para el proyecto MaestrIA · Última actualización: junio 2025*
