# Liz Boutique — cliente

Catálogo de moda (vestidos, zapatos, bolsos y accesorios) con carrito y pedido por WhatsApp. **Cliente** de Zerufy Studio.
**En línea:** https://zerufyx.github.io/LIZ-BOUTIQUE/ (dominio propio pendiente)

| Archivo | Qué es |
|---|---|
| `index.html` | Catálogo: categorías, ofertas, novedades, favoritos, carrito y pedido por WhatsApp |
| `admin.html` | Panel de Liz: productos, fotos, precios, tallas, colores, categorías y ajustes |

**Plan:** pago único de $300, sin mensualidad. Liz sube sus fotos y productos desde el panel.

**Supabase:** sistema de Tiendas, `store_id = 6` (slug `liz-boutique`). Tablas `stores`, `categories`, `products` (usa la columna `colors`). Fotos en el bucket `store-products`, carpeta `6/`. Solo se usa la llave pública.

**WhatsApp, Instagram, Facebook y nota de entrega** se cambian desde el panel (Ajustes). Lo que hay en `CONFIG` dentro de `index.html` solo se usa si el panel no tiene nada guardado.

**Acceso al panel:** la cuenta de Liz se crea en Supabase → Authentication → Add user, y se enlaza con `stores.owner_user_id` de la tienda 6.

---
Hecho por **Zerufy Studio** · zerufystudio.com · El mapa de todos los repos está en el README de `Zerufy-Studio-`.
