# Nutrióloga Herrera — Landing Page

Landing page para la nutrióloga Yessica Yanet Herrera Jiménez (Tulyehualco, Xochimilco, CDMX). Presenta sus servicios de nutrición basada en evidencia —dietas omnívoras, vegetarianas, veganas, keto, sin gluten o sin lactosa, deportivas y para condiciones como diabetes o hipertensión— con planes personalizados y canales directos de contacto (formulario y WhatsApp).

## Stack

- HTML + CSS + JavaScript, sin framework ni paso de build.
- **daisyUI 5 + Tailwind CSS 4** vía CDN (`@tailwindcss/browser@4`).
- Tema personalizado **`nutriologa`** definido en `src/css/global.css` (paleta verde `#2d6a4f`/`#52b788`, acento cálido `#d4a373`, radios y tokens de daisyUI).
- Servidor local con `servor`, despliegue a GitHub Pages con `gh-pages`.

## Estructura

```
src/
├── index.html      # Toda la landing (única página)
├── main.js         # Script actual (mínimo)
└── css/
    └── global.css  # Tema daisyUI "nutriologa" + ajustes base
```

## Secciones (`src/index.html`)

- **Header fijo** (`#header`): `navbar` con avatar/monograma YH, `menu` horizontal en escritorio, CTA "Agenda tu consulta" y `dropdown` hamburguesa en móvil.
- **Hero**: `hero` + `hero-content`, titular, presentación, doble CTA (principal + fantasma) y prueba social con `avatar-group` (+500 pacientes).
- **Sobre mí** (`#sobre-mi`): texto de enfoque profesional, `stats` (8+ años, 500+ pacientes, 100 % evidencia) y `card` de credenciales con `list`/`list-row` y `badge` de áreas.
- **Servicios** (`#servicios`): tres `card` — Consulta Inicial ($800 MXN), Plan Mensual ($2,400 MXN, marcado `Popular`) y Reeducación Alimentaria ($5,500 MXN) — más tarjeta "¿Cómo funciona?" con `steps` de 4 pasos.
- **Modalidades** (`#modalidades`): dos `card` — consulta presencial (Tulyehualco, Xochimilco) y en línea por videollamada para todo México.
- **Testimonios** (`#testimonios`): tres `card` con `rating` de 5 estrellas, cita y `avatar` del paciente.
- **Contacto** (`#contacto`): datos (`list`: dirección y horario Lun–Vie 16:00–21:00), botón directo a WhatsApp (`wa.me/525539355423`) y formulario (`fieldset`, `input`, `textarea`) en `card`.
- **Footer**: `footer` con avatar, aviso de copyright y enlaces sociales.

## Desarrollo

### Prerrequisitos

Asegúrate de tener [Node.js](https://nodejs.org/) y [pnpm](https://pnpm.io/) instalados.

### Servidor local con recarga automática

```bash
pnpm install
pnpm run dev
```

Esto sirve `src/` con `servor` en `http://localhost:1234`.

Otros scripts:

```bash
pnpm start    # servir src/ sin recarga
pnpm preview  # servir src/ y abrir el navegador
```

### Despliegue

```bash
pnpm run deploy
```

Publica `src/` en GitHub Pages con `gh-pages`.
