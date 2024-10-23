### Telegram Media Downloader (Youtube, Twitter and TikTok):

![Telegram Media Downloader Cover](images/ImagenPortada.webp)

**Telegram Media Downloader** is a Python-based bot designed to download videos and audios from platforms like YouTube, Twitter/X, and TikTok. If the file exceeds Telegram's 50 MB limit, it automatically compresses the file using `ffmpeg` and sends it to the user. This bot allows easy downloading and conversion of media through simple commands.

# 🎥 TeleDown Bot

<div align="center">

![GitHub](https://img.shields.io/github/license/tuusuario/teledown-bot)
![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![Telegram](https://img.shields.io/badge/Telegram-Bot-0088cc)

<h3>Bot de Telegram para descargar videos y audio de YouTube, Twitter/X y TikTok</h3>

[Documentación](docs/) |
[Reportar Bug](../../issues) |
[Solicitar Feature](../../issues)

</div>

## 📱 Características

- 📥 Descarga videos de:
  - YouTube
  - Twitter/X
  - TikTok
- 🎵 Extracción de audio en formato MP3
- 📊 Barra de progreso en tiempo real
- 🔄 Conversión automática de formatos
- 💾 Gestión inteligente del almacenamiento temporal
- ⚡ Procesamiento asíncrono para mejor rendimiento

## 🚀 Instalación

1. **Clona el repositorio**
```bash
git clone https://github.com/tuusuario/teledown-bot.git
cd teledown-bot
```

2. **Crea un entorno virtual**
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

3. **Instala las dependencias**
```bash
pip install -r requirements.txt
```

4. **Configura el bot**
- Obtén un token de @BotFather en Telegram
- Crea un archivo `.env` basado en `.env.example`
```env
API_TOKEN=tu_token_aqui
TEMP_DOWNLOAD_FOLDER=/ruta/a/carpeta/temporal
```

5. **Inicia el bot**
```bash
python bot.py
```

## 💡 Uso

### Comandos Disponibles

| Comando | Descripción | Ejemplo |
|---------|-------------|---------|
| `/start` | Inicia el bot y muestra instrucciones | `/start` |
| `/video` | Descarga un video | `/video https://youtube.com/...` |
| `/audio` | Extrae el audio de un video | `/audio https://youtube.com/...` |
| `/help` | Muestra ayuda y comandos disponibles | `/help` |

### Ejemplos de Uso

```plaintext
1. Descargar video de YouTube:
/video https://youtube.com/watch?v=...

2. Extraer audio de video de Twitter:
/audio https://twitter.com/user/status/...

3. Descargar video de TikTok:
/video https://tiktok.com/@user/video/...
```

## ⚙️ Configuración

### Variables de Entorno

| Variable | Descripción | Valor por defecto |
|----------|-------------|-------------------|
| `API_TOKEN` | Token del bot de Telegram | - |
| `TEMP_DOWNLOAD_FOLDER` | Carpeta temporal | `./downloads` |
| `TELEGRAM_MAX_SIZE_MB` | Límite de tamaño | `50` |

## 🛠️ Tecnologías Utilizadas

- **Python 3.8+**
- **python-telegram-bot**: Framework para bots de Telegram
- **yt-dlp**: Librería para descargar contenido multimedia
- **asyncio**: Para operaciones asíncronas

## 📂 Estructura del Proyecto

```
teledown-bot/
├── bot.py              # Código principal del bot
├── requirements.txt    # Dependencias del proyecto
├── .env               # Variables de entorno
├── .gitignore         # Archivos ignorados por git
└── README.md          # Documentación
```

## 🤝 Contribuir

Las contribuciones son bienvenidas. Por favor:

1. Haz un Fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add: nueva característica'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Distribuido bajo la licencia MIT. Ver `LICENSE` para más información.

## ⚠️ Limitaciones

- Tamaño máximo de archivo: 50MB (límite de Telegram)
- Algunos videos pueden no estar disponibles para descarga
- Las descargas dependen de la velocidad de conexión

## 📞 Soporte

- Abre un [issue](../../issues) para reportar bugs
- Únete a nuestro [grupo de Telegram](https://t.me/teledown_support)

---
