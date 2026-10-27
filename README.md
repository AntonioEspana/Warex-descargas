# Warex-descargas

Las versiones publicadas de **Warex para escritorio**: el instalador de Windows y el `latest.json` que lee la aplicación para actualizarse sola.

- **Instalar Warex:** en [Releases](https://github.com/AntonioEspana/Warex-descargas/releases/latest), descarga `Warex_<versión>_x64-setup.exe` y ejecútalo. Como el instalador aún no está firmado, Windows puede decir "Windows protegió su PC": pulsa **Más información** y **Ejecutar de todas formas**. A partir de ahí, Warex se actualiza sola al abrirse.
- **Publicar una versión:** *Actions → Publicar Warex → Run workflow*, con la versión nueva (más alta que la última, p. ej. `0.2.0`). El código está en el repositorio privado de Warex; este solo tiene las releases y el workflow que las construye, porque aquí los minutos de Actions son gratis.

Secretos que necesita el workflow (*Settings → Secrets and variables → Actions*): `WAREX_CODE_TOKEN` (token con *Contents: Read-only* en `AntonioEspana/Warex`) y `TAURI_SIGNING_PRIVATE_KEY` (la clave privada del actualizador).
