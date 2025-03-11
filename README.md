# Carrousel de Imágenes (banner principal)

### Archivo: home-slider.tpl

### settings.txt:
```txt
collapse
    title = Carrusel de imágenes
    backto = home_order_position
checkbox
    name = slider_animation
    description = Agregar efecto de movimiento a las imágenes del carrusel
subtitle
    subtitle = Imágenes para computadoras
gallery
    name = slider
    gallery_image = Agregar imagen
    gallery_link = [Opcional] Página web a la que quieres que te lleve la imagen al hacer click
    gallery_width = 1580
    gallery_height = 600
    gallery_more_info = true
subtitle
    subtitle = Imágenes para celulares
description
    description = Mejorá la calidad y velocidad de carga con esta opción
checkbox
    name = toggle_slider_mobile
    description = Cargar otras imágenes para celulares
gallery
    name = slider_mobile
    gallery_image = Agregar imagen
    gallery_link = [Opcional] Página web a la que quieres que te lleve la imagen al hacer click
    gallery_width = 820
    gallery_height = 1200
    gallery_more_info = true
subtitle
    subtitle = <a target='_blank' data-toggle-info='show-on_slider_mobile-inactive' href='https://ayuda.tiendanube.com/es/articles/3297783-como-usar-el-carrusel-de-imagenes-para-las-plantillas-idea-bahia-y-amazonas'>¿Cómo diseñar las imágenes para tu carrusel?</a>
```
### Ejemplo como llamar datos en .TPL: {{settings.slider}}

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/carrousel_de_imágenes.png)


# Carrousel de Productos (Nuevos,Destacados,Oferta) (Grilla o Carrusel)

### Archivo: home-featured-grid.tpl

### settings.txt:

```txt
collapse
    title = Productos destacados
    backto = home_order_position
i18n_input
    name = featured_products_title
    description = Título para los productos destacados
dropdown
    name = featured_products_format
    description = Mostrar los productos como:
    values
        grid = Grilla
        slider = Carrusel
title
    title = Disposición en celulares
dropdown
    name = featured_products_mobile
    description = Cantidad de productos por fila
    values
        default = Misma cantidad que en el listado de productos
        1 = 1 producto
        2 = 2 productos
        3 = 3 productos
subtitle
    subtitle = <span class='legend'>Al elegir 3 se mostrarán sólo el precio y la imagen de los productos</span>
title
    title = Disposición en computadoras
dropdown
    name = featured_products_desktop
    description = Cantidad de productos por fila
    values
        default = Misma cantidad que en el listado de productos
        2 = 2 productos
        3 = 3 productos
        4 = 4 productos
```

### Ejemplo como llamar datos en .TPL: {{settings.featured_products_title}}

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/carrousel_de_productos.png)


# Video (Autoplay)

### Archivo: home-video.tpl

### settings.txt:

```txt
collapse
    title = Video
    backto = home_order_position
i18n_input
    name = texto__video
    description = Texto
dropdown
    name = video_type
    description = Tipo de reproducción
    values
        autoplay = Automática y sin sonido
        sound = Con sonido y sin reproducción automática
i18n_input
    name = video_embed
    description = Link de YouTube
description
    description = Ej: https://www.youtube.com/watch?v=Yn19Od1H0S4
subtitle
    subtitle = Imagen del video
description
    description = No aplica si el tipo de reproducción es automática y el video no está en la primera posición
image
    original = video_image.jpg
    title = Cargar imagen (JPG, GIF, PNG)
    width = 1280
    height = 720
i18n_input
    name = video_title
    description = Título
i18n_input
    name = video_subtitle
    description = Subtítulo
i18n_input
    name = video_text
    description = Descripción
i18n_input
    name = video_button
    description = Texto del botón
i18n_input
    name = video_button_url
    description = Link del botón
checkbox
    name = video_vertical_mobile
    description = Usar formato vertical en celulares
```

### Ejemplo como llamar datos en .TPL: {{settings.texto__video}}

![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/video.gif)

# Módulo de imagen y texto 

### Archivo: home-banners-grid.tpl

### settings.txt:

```txt
collapse
    title = Módulos de imagen y texto
    backto = home_order_position
description
    description = Podés cargar los módulos que necesites, sin límite de cantidad.
checkbox
    name = module_slider
    description = Mostrar los módulos dentro de un carrusel
checkbox
    name = module_same_size
    description = Usar el mismo alto para todos los módulos
gallery
    name = module
    gallery_image = Agregar imagen
    gallery_link = [Opcional] Página web a la que quieres que te lleve la imagen al hacer click
    gallery_width = 1920
    gallery_height = 900
    gallery_more_info = true
```

### Ejemplo como llamar datos en .TPL: {% set section_banner = settings.module %}

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/modulo_imagen_y_texto.png)


# Mensaje institucional

### Archivo: 

### settings.txt: home-welcome-message.tpl

```txt
collapse
    title = Mensaje institucional
    backto = home_order_position
i18n_input
    name = welcome_message
    description = Título
i18n_input
    name = welcome_text
    description = Descripción
```

### Ejemplo como llamar datos en .TPL: {{ settings.welcome_text }}

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/custom_message.png)


# Banners Promocionales / Banner Novedades / Banner Categorías

### Archivo: home-banners-grid.tpl

### settings.txt:

```txt
collapse
    title = Banners promocionales
    backto = home_order_position
description
    description = Podés cargar los banners que necesites, sin límite de cantidad.
checkbox
    name = banner_promotional_text_outside
    description = Mostrar texto fuera de la imagen
checkbox
    name = banner_promotional_slider
    description = Mostrar banners dentro de un carrusel
checkbox
    name = banner_promotional_same_size
    description = Usar el mismo alto para todos los banners
subtitle
    subtitle = Imágenes para computadoras
dropdown
    name = banner_promotional_columns_desktop
    description = Disposición de banners en computadoras
    values
        1 = 1 banner por fila
        2 = 2 banners por fila
        3 = 3 banners por fila
        4 = 4 banners por fila
gallery
    name = banner_promotional
    gallery_image = Agregar imagen
    gallery_link = [Opcional] Página web a la que quieres que te lleve la imagen al hacer click
    gallery_width = 930
    gallery_height = 465
    gallery_more_info = true
subtitle
    subtitle = Imágenes para celulares
dropdown
    name = banner_promotional_columns_mobile
    description = Disposición de banners en celulares
    values
        1 = 1 banner por fila
        2 = 2 banners por fila
checkbox
    name = toggle_banner_promotional_mobile
    description = Cargar otras imágenes para celulares
gallery
    name = banner_promotional_mobile
    gallery_image = Agregar imagen
    gallery_link = [Opcional] Página web a la que quieres que te lleve la imagen al hacer click
    gallery_width = 820
    gallery_height = 1000
    gallery_more_info = true
```

### Ejemplo como llamar datos en .TPL: 

### Imagen Ejemplo:{% set has_banners = settings.banner_promotional and settings.banner_promotional is not empty %}
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/banners_categorias.png)


# Newsletter

### Archivo: home-newsletter.tpl

### settings.txt:

```txt
	collapse
		title = Newsletter
		backto = home_order_position
	checkbox
		name = home_news_colors
		description = Usar estos colores para el newsletter
	color
		name = home_news_background_color
		description = Color de fondo
	color
		name = home_news_foreground_color
		description = Color de textos
	description
		description = Imagen
	image
		original = home_news_image.jpg
		title = Cargar imagen (JPG, GIF, PNG)
		width = 1920
		height = 480
	description
		description = Imagen para celulares (opcional)
	image
		original = home_news_image_mobile.jpg
		title = Cargar imagen (JPG, GIF, PNG)
		width = 820
		height = 820
	dropdown
		name = home_news_align
		description = Alineación del texto
		values
			left = Izquierda
			center = Centrado
	i18n_input
		name = home_news_title
		description = Título
	i18n_input
		name = home_news_text
		description = Descripción
```

### Ejemplo como llamar datos en .TPL: settings.home_news_align

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/newsletter.png)


# Marcas

### Archivo: home-brands.tpl

### settings.txt:

```txt
	collapse
		title = Marcas
		backto = home_order_position
	i18n_input
		name = brands_title
		description = Título
	gallery
		name = brands
		gallery_image = Agregar imagen
		gallery_link = [Opcional] Página web a la que quieres que te lleve la imagen al hacer click
		gallery_width = 200
		gallery_height = 200
```

### Ejemplo como llamar datos en .TPL:  {{settings.brands}}

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/nuestras_marcas.png)



# Testimonios

### Archivo: home-testimonials.tpl

### settings.txt:

```txt
collapse
    title = Testimonios
    backto = home_order_position
i18n_input
    name = testimonials_title
    description = Título
subtitle
    subtitle = Testimonio 1
image
    original = testimonial_01.jpg
    title = Cargar imagen (JPG, GIF, PNG)
    width = 180
    height = 180
i18n_input
    name = testimonial_01_description
    description = Descripción
i18n_input
    name = testimonial_01_name
    description = Nombre
subtitle
    subtitle = Testimonio 2
image
    original = testimonial_02.jpg
    title = Cargar imagen (JPG, GIF, PNG)
    width = 180
    height = 180
i18n_input
    name = testimonial_02_description
    description = Descripción
i18n_input
    name = testimonial_02_name
    description = Nombre
subtitle
    subtitle = Testimonio 3
image
    original = testimonial_03.jpg
    title = Cargar imagen (JPG, GIF, PNG)
    width = 180
    height = 180
i18n_input
    name = testimonial_03_description
    description = Descripción
i18n_input
    name = testimonial_03_name
    description = Nombre
```

### Ejemplo como llamar datos en .TPL: {{ settings.testimonials_title }}

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/testimonials.png)



# Categorias principales (imagenes chicas)

### Archivo: home-categories.tpl

### settings.txt:

```txt
collapse
    title = Categorías principales
    backto = home_order_position
checkbox
    name = main_categories
    description = Mostrar categorías en la página principal
gallery
    name = slider_categories
    gallery_image = Agregar imagen
    gallery_link = [Opcional] Página web a la que quieres que te lleve la imagen al hacer click
    gallery_width = 120
    gallery_height = 120

```

### Ejemplo como llamar datos en .TPL: {{ settings.slider_categories }}

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/categorias_chicas.png)



# Información de envíos, pagos y compra

### Archivo: snipplets > banner-services (dos archivos)

### settings.txt:

```txt
collapse
    title = Información de envíos, pagos y compra
    backto = home_order_position
checkbox
    name = banner_services
    description = Mostrar los banners en la página principal
subtitle
    subtitle = BANNER 1
image
    original = banner_services_01.jpg
    title = Cargar imagen (JPG, GIF, PNG)
    width = 600
    height = 600
dropdown
    name = banner_services_01_icon
    description = Ícono
    values
        image = Imagen propia
        shipping = Envíos
        card = Tarjetas de crédito
        security = Seguridad
        returns = Cambios y devoluciones
        whatsapp = WhatsApp
        promotions = Promociones
        cash = Pago en efectivo
i18n_input
    name = banner_services_01_title
    description = Título
i18n_input
    name = banner_services_01_description
    description = Descripción
i18n_input
    name = banner_services_01_url
    description = Link
subtitle
    subtitle = BANNER 2
image
    original = banner_services_02.jpg
    title = Cargar imagen (JPG, GIF, PNG)
    width = 600
    height = 600
dropdown
    name = banner_services_02_icon
    description = Ícono
    values
        image = Imagen propia
        shipping = Envíos
        card = Tarjetas de crédito
        security = Seguridad
        returns = Cambios y devoluciones
        whatsapp = WhatsApp
        promotions = Promociones
        cash = Pago en efectivo
i18n_input
    name = banner_services_02_title
    description = Título
i18n_input
    name = banner_services_02_description
    description = Descripción
i18n_input
    name = banner_services_02_url
    description = Link
subtitle
    subtitle = BANNER 3
image
    original = banner_services_03.jpg
    title = Cargar imagen (JPG, GIF, PNG)
    width = 600
    height = 600
dropdown
    name = banner_services_03_icon
    description = Ícono
    values
        image = Imagen propia
        shipping = Envíos
        card = Tarjetas de crédito
        security = Seguridad
        returns = Cambios y devoluciones
        whatsapp = WhatsApp
        promotions = Promociones
        cash = Pago en efectivo
i18n_input
    name = banner_services_03_title
    description = Título
i18n_input
    name = banner_services_03_description
    description = Descripción
i18n_input
    name = banner_services_03_url
    description = Link

```

### Ejemplo como llamar datos en .TPL: {{ settings.banner_services_01_title }}

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/tira_informativa.png)



# Producto principal (Destacar un item)

### Archivo: home-main-product.tpl

### settings.txt:

```txt
	collapse
		title = Producto principal
		backto = home_order_position
	description
		description = Se va a mostrar un solo producto de la sección 'Principal'.
	dropdown
		name = main_product_type
		description = Mostrar:
		values
			first = El primero de la lista
			random = En forma aleatoria
	subtitle
		subtitle = <a target='_blank' href='/admin/themes/settings/product_order/'>Elegí cuál vas a destacar</a>
```

### Ejemplo como llamar datos en .TPL: {% set product_type = sections.featured.products | take(1) %}

### Imagen Ejemplo:
![Imagen de ejemplo](https://www.recursosindex.com/recursos/modulos_tn/destacar_un_item.png)


