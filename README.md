# Aracari App · releases

Instaladores y actualizaciones de **Aracari App** para macOS (universal) y Windows.

Este repositorio es público a propósito: la app instalada consulta aquí `latest.json` para detectar y aplicar
actualizaciones sin credenciales. El código fuente está en un repositorio privado y no se publica aquí.

| Archivo | Uso |
|---|---|
| `Aracari_X.Y.Z_universal.dmg` | Instalar en macOS |
| `Aracari_X.Y.Z_x64-setup.exe` | Instalar en Windows (por usuario, sin permisos de administrador) |
| `Aracari_X.Y.Z_x64_en-US.msi` | Despliegue corporativo en Windows |
| `latest.json`, `*.sig`, `*.tar.gz` | Los usa la app para actualizarse (no hace falta descargarlos) |

La app aún no está firmada con certificados de Apple ni de Microsoft: la primera vez, macOS pide *Ajustes →
Privacidad y seguridad → Abrir igualmente* y Windows muestra SmartScreen (*Más información → Ejecutar de todas formas*).
Las actualizaciones posteriores no muestran estos avisos.

Los releases se publican con el workflow **Release** (Actions) o con `scripts/release.sh` del repositorio privado.
