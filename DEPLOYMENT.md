# 🚀 Guía de Despliegue - Quiniela Liga MX

Esta guía te ayudará a desplegar la aplicación Quiniela Liga MX en producción.

## ✅ Pre-requisitos

- La aplicación está lista para desplegar
- El código está en GitHub
- Tienes acceso de administrador al repositorio

## 📋 Pasos para Desplegar en GitHub Pages

### 1. Activar GitHub Pages

1. Abre tu repositorio en GitHub: `https://github.com/Joseluiscruz-hub/Quiniela-TAB`
2. Ve a **Settings** (Configuración) en la parte superior
3. En el menú lateral, selecciona **Pages**
4. En la sección **Build and deployment**:
   - **Source**: Selecciona **GitHub Actions**
   
   ![GitHub Pages Settings](https://docs.github.com/assets/cb-47267/mw-1440/images/help/pages/pages-source-github-actions.webp)

5. Haz clic en **Save** (Guardar)

### 2. Verificar el Despliegue

1. Ve a la pestaña **Actions** en tu repositorio
2. Verás un workflow llamado "Deploy to GitHub Pages" ejecutándose
3. Espera a que el workflow termine (aprox. 1-2 minutos)
4. Una vez completado, verás un mensaje de éxito con la URL de tu sitio

### 3. Acceder a tu Aplicación

Tu aplicación estará disponible en:
```
https://joseluiscruz-hub.github.io/Quiniela-TAB/
```

## 🔄 Actualizaciones Automáticas

La aplicación se desplegará automáticamente cada vez que:
- Hagas merge de un Pull Request a `main`
- Hagas push directo a `main`
- Hagas push a `copilot/accept-changes-and-launch-app`

## 🛠️ Despliegue Manual

Si necesitas redesplegar la aplicación manualmente:

1. Ve a la pestaña **Actions**
2. Selecciona **Deploy to GitHub Pages** en la lista de workflows
3. Haz clic en el botón **Run workflow** (▶️)
4. Selecciona la rama desde la que deseas desplegar
5. Haz clic en **Run workflow**

## 🔍 Verificación de Funcionalidad

Una vez desplegada, verifica que:

- [ ] La página carga correctamente
- [ ] El contador de tiempo está funcionando
- [ ] Puedes seleccionar pronósticos para cada partido
- [ ] La barra de progreso se actualiza al seleccionar partidos
- [ ] El formulario de datos personales funciona
- [ ] El botón de envío está habilitado

## ⚡ Despliegue Local (Para Pruebas)

Si quieres probar la aplicación localmente antes de desplegar:

```bash
# Con Python
python3 -m http.server 8080

# Con Node.js
npx http-server

# Con PHP
php -S localhost:8080
```

Luego abre `http://localhost:8080` en tu navegador.

## 🐛 Solución de Problemas

### El workflow falla con "action_required"

**Solución**: Asegúrate de haber habilitado GitHub Pages en Settings → Pages y seleccionado "GitHub Actions" como fuente.

### La página muestra un error 404

**Solución**: 
1. Verifica que el archivo `index.html` esté en la raíz del repositorio
2. Espera unos minutos después del despliegue (puede tomar hasta 10 minutos)
3. Limpia la caché de tu navegador

### El workflow se ejecuta pero no veo mi sitio

**Solución**:
1. Ve a Settings → Pages
2. Verifica que veas la URL de tu sitio publicado
3. Si no aparece, intenta ejecutar el workflow manualmente

## 📞 Soporte

Si tienes problemas con el despliegue:

1. Revisa los logs del workflow en la pestaña Actions
2. Verifica que todos los archivos necesarios estén en el repositorio
3. Asegúrate de tener los permisos correctos en el repositorio

## 🎉 ¡Listo!

Una vez completados estos pasos, tu aplicación Quiniela Liga MX estará disponible para todos los usuarios.

---

**Nota**: El despliegue en GitHub Pages es completamente gratuito y no requiere configuración de servidor.
