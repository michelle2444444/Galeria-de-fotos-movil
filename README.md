# Galeria-de-fotos-movil

1.- Mostrar las fotos y además mostrar el nombre del archivo debajo de cada foto.

📸 Antes: Las fotos se mostraban, pero no sabías su nombre de archivo.

🛠️ Ahora: Cada foto guardada se presenta con su ruta o nombre de archivo (por ejemplo: 1683548324563.jpeg) justo debajo de la imagen.

📍¿Dónde ocurre esto?
En tab3.page.html, dentro de cada tarjeta (ion-card) que contiene la foto, se agrega un párrafo con {{ photo.filepath }}.

🔍 ¿Para qué sirve?

Útil para identificar las fotos por nombre.

![image](https://github.com/user-attachments/assets/0710ec26-99d8-4638-b7b6-8cb5b1383351)

2.- Mostrar las fotos previamente guardadas en el tab3 en lugar del tab2

📍Antes: Todas las fotos se tomaban y se mostraban en el Tab 2 (la misma vista).

📍Ahora:

Tab 2: solo tiene los botones para capturar nuevas fotos (100% o 50% de calidad).

Tab 3: es el lugar donde puedes ver las fotos ya guardadas.

🧠 Beneficio: Separar las funcionalidades:

Tab 2: entrada de datos (captura).

Tab 3: salida de datos (visualización).

![image](https://github.com/user-attachments/assets/a668110b-0942-4511-9368-af4de3013713)

3.- No mostrar las fotos automáticamente, implementar un botón que me permita cargar las fotos (en cualquier tab).

🔁 Antes: Las fotos se cargaban automáticamente al entrar al tab usando ngOnInit.

⏯️ Ahora: Ya no se cargan automáticamente.

Se debe hacer clic en "Cargar Fotos" para verlas.

🛠️ Esto se implementa con un botón en tab3.page.html que llama al método loadPhotos().

🎯 ¿Por qué es útil?

Más control del usuario y ahorra recursos (no carga imágenes innecesariamente).

Ideal si en el futuro agregas filtros o múltiples fuentes de imágenes.

![image](https://github.com/user-attachments/assets/cfa29646-dcc9-4279-a813-5b6b771f030d)

4.- Implementar un botón adicional que tome las fotos al 50% de calidad.

📷 Antes: Solo podías tomar fotos con calidad máxima (100%).

➕ Ahora: Existe la opcion de tomar fotos con calidad media (50%).

🛠️ Se implementa en tab2.page.html

🧠 ¿Para qué sirve?

Las fotos de calidad 50% usan menos espacio. Útil si el usuario necesita muchas fotos y quiere ahorrar memoria o subirlas más rápido.

![image](https://github.com/user-attachments/assets/03bf2608-577f-469b-8124-ad2c60c18943)

| Tab   | Función Principal              | Interacción Principal    |
| ----- | ------------------------------ | ------------------------ |
| Tab 2 | Capturar fotos (100% y 50%)    | Botones `camera` y `50%` |
| Tab 3 | Ver fotos guardadas con nombre | Botón `Cargar Fotos`     |



