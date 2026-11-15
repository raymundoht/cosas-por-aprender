# Ruleta del Saber

Una ruleta que te da un tema al azar para investigar. Cada tema sale **una sola vez**. Lo que ya salió y los temas que agregues se guardan en `datos.json`, dentro de este repositorio, así que se respetan en cualquier navegador.

## Ponerla en línea (una sola vez)

1. Crea un repositorio nuevo en GitHub (por ejemplo `ruleta`) y sube `index.html`, `datos.json` y este `README.md`.
2. En el repositorio, entra a **Settings → Pages**. En «Source» elige **Deploy from a branch**, rama **main**, carpeta **/ (root)**, y guarda.
3. Después de uno o dos minutos, la ruleta queda en `https://TU-USUARIO.github.io/ruleta/`.

## Crear el token (una sola vez)

Con el token, la página puede guardar cambios en `datos.json`.

1. En GitHub: tu foto → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. En **Repository access** elige **Only select repositories** y selecciona solo el repositorio de la ruleta.
3. En **Permissions → Repository permissions → Contents**, elige **Read and write**.
4. Genera el token y cópialo. GitHub solo lo muestra una vez.

## Conectar cada navegador

Abre la ruleta, pulsa **⚙ GitHub**, pega el token y pulsa **Guardar y probar**. Si la abres desde `github.io`, el usuario y el repositorio se llenan solos. Esto se hace una vez en cada navegador o computadora.

Cuando abajo dice **● Sincronizado con GitHub**, todo se guarda en el repositorio.

## Cómo funciona

- **Girar:** el tema que sale se elimina y no vuelve a salir, ni en este navegador ni en otro.
- **+ Agregar tema:** escribe un tema que se te ocurra. Queda escondido y te saldrá algún día al azar. Cuando sale, se borra.
- **Reiniciar:** los temas de la lista pueden volver a salir. Los temas que tú agregaste y ya salieron no regresan.

Cada vez que giras o agregas un tema, la página hace un commit en `datos.json`. Los temas se guardan codificados, para que no los leas por accidente al abrir el archivo.

**Seguridad:** el token solo tiene permiso sobre este repositorio y se guarda únicamente en los navegadores donde lo pegas. No lo compartas. Si crees que alguien lo vio, bórralo en GitHub y crea otro.
