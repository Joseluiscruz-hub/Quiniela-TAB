# 🏆 Quiniela Liga MX

Aplicación web para gestionar quinielas de la Liga MX - Clausura 2025.

## 📋 Descripción

Esta es una aplicación web moderna y responsive para crear y participar en quinielas de fútbol de la Liga MX. Los usuarios pueden:

- ✅ Hacer pronósticos de los 9 partidos de la jornada
- 📊 Ver su progreso en tiempo real
- ⏰ Contar con un temporizador de cuenta regresiva hasta la fecha límite
- 💾 Guardar automáticamente sus pronósticos en el navegador
- 📱 Usar la aplicación desde cualquier dispositivo (diseño responsive)

## 🚀 Despliegue

### GitHub Pages

La aplicación está lista para desplegarse en GitHub Pages:

1. Ve a Settings → Pages
2. En "Source", selecciona la rama principal
3. Guarda los cambios
4. La aplicación estará disponible en: `https://joseluiscruz-hub.github.io/Quiniela-TAB/`

### Despliegue Local

Para probar la aplicación localmente:

```bash
# Opción 1: Python
python3 -m http.server 8080

# Opción 2: Node.js
npx http-server

# Luego abre http://localhost:8080 en tu navegador
```

## ⚙️ Configuración

La aplicación está pre-configurada con:

- **Google Script URL**: Conectado para guardar las quinielas
- **Fecha límite**: 10 de enero de 2026, 18:00
- **Total de partidos**: 9
- **Premios**:
  - 1er lugar: $1,000 MXN
  - 2do lugar: $500 MXN
  - 3er lugar: $500 MXN

## 🎯 Características

- 🎨 Diseño moderno con tema oscuro
- ⚡ Sin dependencias externas (vanilla JavaScript)
- 💾 Guardado automático en localStorage
- 📱 Completamente responsive
- ✨ Animaciones suaves y efectos visuales
- 🔔 Notificaciones toast para feedback del usuario
- ✅ Validación de formularios
- ⏱️ Contador de tiempo en vivo

## 📦 Estructura

```
Quiniela-TAB/
├── index.html          # Aplicación principal (HTML + CSS + JS)
└── README.md          # Este archivo
```

## 🛠️ Tecnologías

- HTML5
- CSS3 (Variables CSS, Grid, Flexbox)
- JavaScript (ES6+)
- Google Apps Script (backend)

## 📝 Licencia

© 2025 Quiniela Liga MX - Todos los derechos reservados

---

Desarrollado con ❤️ para aficionados del fútbol mexicano
