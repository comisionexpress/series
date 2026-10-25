# Del libro a la serie

Webapp que lee el PDF de un libro y planifica la serie: análisis de adaptabilidad, episodios, escenas y planos con prompts para Google Flow y voz en off para ElevenLabs.

## Publicarla en GitHub Pages (sin instalar nada)

1. En github.com, crear un repositorio nuevo, por ejemplo `motor-de-series`.
2. Entrar en **Add file → Upload files**, subir `index.html` y `README.md`, y confirmar con **Commit changes**.
3. Ir a **Settings → Pages**. En **Source** elegir **Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guardar.
4. Esperar uno o dos minutos. La web queda en `https://TU-USUARIO.github.io/motor-de-series/`.

## Primer uso

1. Abrir la web y, en **Conexión con Claude**, pegar la clave de API de Anthropic (se crea en console.anthropic.com, sección API keys).
2. Cargar el PDF, completar autor y confirmar la autorización del autor.
3. Seguir los pasos: analizar el libro, armar la temporada y generar los planos.

## Importante

- La clave se guarda solo en el navegador de quien la pega (localStorage) y se envía únicamente a Anthropic. No queda en el repositorio.
- Cada persona que abra la web tiene que usar su propia clave. No compartas tu clave con colegas.
- Cada paso que lee el PDF consume tokens de la cuenta de la clave usada.
- Los proyectos se guardan en el navegador del dispositivo. Para pasarlos a otro dispositivo, usar **Descargar proyecto (.json)** e **Importar proyecto**.
- Si más adelante se quiere ofrecer la herramienta a clientes sin que carguen su propia clave, hace falta un servidor intermedio que guarde la clave de forma segura.
