# Warex-descargas

Las versiones publicadas de **Warex para escritorio**: los instaladores de Windows y de Linux y el `latest.json` que lee la aplicación para actualizarse sola.

- **Instalar Warex en Windows:** en [Releases](https://github.com/AntonioEspana/Warex-descargas/releases/latest), descarga `Warex_<versión>_x64-setup.exe` y ejecútalo. Como el instalador aún no está firmado, Windows puede decir "Windows protegió su PC": pulsa **Más información** y **Ejecutar de todas formas**. A partir de ahí, Warex se actualiza sola al abrirse.
- **Instalar Warex en Linux** (64 bits), desde la misma release:
  - **Ubuntu, Debian, Mint y derivadas:** descarga `Warex_<versión>_amd64.deb` e instálalo con doble clic o con `sudo apt install ./Warex_<versión>_amd64.deb`. Al actualizarse, el sistema pide la contraseña.
  - **Cualquier otra distribución:** descarga `Warex_<versión>_amd64.AppImage`, dale permiso de ejecución (`chmod +x Warex_*.AppImage`) y ábrelo. Se actualiza solo, sin contraseña.
- **Publicar una versión:** *Actions → Publicar Warex → Run workflow*, con la versión nueva (más alta que la última, p. ej. `0.2.0`). El código está en el repositorio privado de Warex; este solo tiene las releases y el workflow que las construye, porque aquí los minutos de Actions son gratis.

Secretos que necesita el workflow (*Settings → Secrets and variables → Actions*): `WAREX_CODE_TOKEN` (token con *Contents: Read-only* en `AntonioEspana/Warex`) y `TAURI_SIGNING_PRIVATE_KEY` (la clave privada del actualizador).
