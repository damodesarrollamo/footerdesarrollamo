# Footer Service DesarrollAMO

**URL:** https://damodesarrollamo.github.io/footerdesarrollamo/

## Cómo usarlo en cualquier sitio

### Opción 1: Script tag (recomendado)
```html
<div id="da-footer"></div>
<script>
(function() {
  var s = document.createElement('script');
  s.src = 'https://damodesarrollamo.github.io/footerdesarrollamo/?name=NOMBRE&slogan=SLOGAN&theme=light';
  s.onload = function() { document.getElementById('da-footer').innerHTML = document.body.innerHTML; document.body.innerHTML = '';
};
  document.head.appendChild(s);
})();
</script>
```

### Opción 2: Copiar HTML directo (más rápido para 90 sitios)
Usar el contenido de `footer-embed.html` (copiar/pegar en cada proyecto)

## Parámetros
- `name` — Nombre del cliente (ej: "CasaBosco")
- `slogan` — Actividad (ej: "Arquitectura & Diseño")
- `theme` — "light" | "dark"
- `credit` — Texto de crédito personalizado

## Colores oficiales DesarrollAMO
- Celeste (Desarroll): `#79D7ED`
- Rosa (AMO): `#E287B2`
- Dorado (Sol): `#F2B077`

## Para agregar nuevos sitios al config
Editar `index.html` y agregar en `SITE_CONFIG`:
```js
'sitio.com': { name: 'Cliente', slogan: 'Actividad', theme: 'light' }
```