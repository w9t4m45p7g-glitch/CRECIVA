# CRECIVA: guía para publicar la aplicación

Contenido: `index.html` (la app), `manifest.webmanifest` + `sw.js` + iconos (instalable y funciona sin internet), `privacidad.html` y `terminos.html`.

## Opción A: Netlify (la más rápida, ~5 min)
1. Entra a netlify.com y crea una cuenta gratuita (verifica en su sitio si el plan gratis sigue vigente).
2. En "Add new site" elige "Deploy manually" y arrastra la carpeta completa del paquete.
3. Te dará un enlace público. Ábrelo en tu celular: en Chrome usa "Instalar aplicación" o "Añadir a pantalla de inicio".

## Opción B: GitHub Pages
1. Crea un repositorio público y sube los archivos.
2. Settings > Pages > Deploy from a branch > main / root.

## Dominio propio (opcional)
Un dominio .co o .com tiene un costo anual (cotízalo en el registrador). Antes de comprarlo, verifica disponibilidad de "creciva".

## Antes de difundirla: pendientes humanos
- [ ] Reemplazar los textos amarillos [RAZÓN SOCIAL], [NIT], [DIRECCIÓN], [CORREO], [FECHA] en `privacidad.html` y `terminos.html`. Mientras la empresa no esté constituida, no publiques datos que no existan: usa los de la persona natural responsable o espera a constituirla.
- [ ] Que un abogado revise la política y los términos. Son un borrador de buena fe, no asesoría jurídica.
- [ ] Consultar "CRECIVA" en SIPI (sipi.sic.gov.co), clases 9, 35, 36 y 42, y guardar capturas. No hay verificación de disponibilidad hecha.
- [ ] Probar en Android, iPhone y computador.

## Registro Nacional de Bases de Datos (RNBD)
Según el Decreto 090 de 2018, solo están obligadas a inscribirse las sociedades y entidades sin ánimo de lucro con activos totales superiores a 100.000 UVT, además de las entidades públicas. Una empresa nueva y pequeña normalmente queda fuera, pero sigue obligada a cumplir la Ley 1581 (política, autorización, atención de reclamos). Confirma con un asesor.

## Para activar cuentas y nube (versión 2)
Hoy la app NO tiene cuentas: todo queda en el dispositivo. Para tener cuentas reales se requiere un servicio de base de datos con autenticación (por ejemplo Supabase o Firebase), programar el inicio de sesión y reglas de acceso por usuario, y probarlo. Al activarlo hay que actualizar `privacidad.html`, pedir autorización previa expresa antes de recolectar datos, definir un canal para reclamos y un plan de respuesta a incidentes de seguridad, y revisar si aplica el RNBD.

## App Store y Google Play
Esta es una app web instalable (PWA). Publicarla en tiendas exige cuentas de desarrollador de pago y empaquetarla; no es necesario para el piloto.
