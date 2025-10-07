<div align="center">

# 🏭 RELY Node-RED Nodes

### Catálogo de Nodos Industriales

[![Packages](https://img.shields.io/badge/packages-23-27ae60.svg)](https://github.com/orgs/Sialitech/packages)
[![Node-RED](https://img.shields.io/badge/Node--RED-Compatible-c0392b.svg)](https://nodered.org)

[🌐 Documentación Completa](https://sialitech.github.io/rely-docs/) • [📦 Ver Paquetes](https://github.com/orgs/Sialitech/packages)

</div>

---

## 📋 Contenido de esta Carpeta

Este directorio contiene la documentación pública para usuarios finales de RELY Node-RED Nodes:

- **`index.html`** - Página web principal con guía de instalación
- **`rely-catalogue.json`** - Catálogo para Node-RED (configurar en `settings.js`)
- **`README.md`** - Este archivo

---

## 🚀 Instalación Rápida

### 1. Obtener Token de Acceso

Genera un **Personal Access Token** en GitHub con permiso `read:packages`:

👉 [github.com/settings/tokens/new](https://github.com/settings/tokens/new)

### 2. Configurar Acceso

```bash
cd ~/.node-red

cat > .npmrc << 'NPMRC'
@sialitech:registry=https://npm.pkg.github.com
//npm.pkg.github.com/:_authToken=TU_TOKEN_AQUI
NPMRC
```

### 3. Instalar Bundle Completo

```bash
npm install @sialitech/node-red-contrib-rely-bundle
```

✅ Instala **22 nodos industriales** automáticamente

### 4. Reiniciar Node-RED

```bash
node-red-stop
node-red-start
```

---

## 📦 Paquetes Disponibles

### Total: 23 paquetes

- **1 Bundle** (meta-paquete que instala todos)
- **22 Nodos** individuales

### Por Categoría

| Categoría | Cantidad | Nodos |
|-----------|----------|-------|
| 🎥 **Visión e Imágenes** | 7 | camara-pycam, camara-simulada, images, yolo, vision-tradicional, medidas, ocr |
| 🔍 **Control de Calidad** | 4 | anomalias, presencias, receta, contaje |
| 🏷️ **Identificación** | 2 | lector-codigos, id-manufacturer |
| ⚙️ **Control Industrial** | 4 | read-signal, write-signal, relay, marcha |
| 💾 **Gestión de Datos** | 5 | sql-puzzle, proyecto, referencia, gestor, meta |

---

## 🎨 Mostrar en la Paleta de Node-RED

Edita `~/.node-red/settings.js`:

```javascript
module.exports = {
    editorTheme: {
        palette: {
            catalogues: [
                'https://catalogue.nodered.org/catalogue.json',
                'https://sialitech.github.io/rely-docs/rely-catalogue.json'
            ]
        }
    }
}
```

Reinicia Node-RED y busca `@sialitech` en la paleta.

---

## 💡 Instalación Selectiva

También puedes instalar solo los nodos que necesites:

```bash
# Visión artificial
npm install @sialitech/node-red-contrib-yolo
npm install @sialitech/node-red-contrib-medidas
npm install @sialitech/node-red-contrib-ocr

# Control de calidad
npm install @sialitech/node-red-contrib-anomalias
npm install @sialitech/node-red-contrib-presencias

# Control PLC
npm install @sialitech/node-red-contrib-read-signal
npm install @sialitech/node-red-contrib-write-signal
```

---

## 🔄 Actualización

### Actualizar todos los nodos

```bash
cd ~/.node-red
npm update @sialitech/*
```

### Actualizar solo el bundle

```bash
npm update @sialitech/node-red-contrib-rely-bundle
```

---

## 📖 Documentación Completa

Visita la documentación web para:

- 📋 Lista detallada de todos los nodos
- 📝 Ejemplos de uso
- 🔧 Configuración avanzada
- 🐛 Solución de problemas

👉 **https://sialitech.github.io/rely-docs/**

---

## 🔗 URL del Catálogo

El catálogo JSON está disponible públicamente en:

```
https://sialitech.github.io/rely-docs/rely-catalogue.json
```

Este archivo se actualiza **automáticamente** cada vez que se publican nuevas versiones.

---

## 🐛 Solución de Problemas

### Los nodos no aparecen en Node-RED

**Solución:** Verifica que el archivo `.npmrc` esté en `~/.node-red/` y reinicia Node-RED completamente.

### Error: "401 Unauthorized"

**Solución:** Tu token no tiene permisos o ha expirado. Genera uno nuevo con `read:packages`.

### Error al instalar

**Solución:** Verifica que el `.npmrc` tenga el formato correcto:

```
@sialitech:registry=https://npm.pkg.github.com
//npm.pkg.github.com/:_authToken=ghp_...
```

---

## 📞 Soporte

Para solicitar acceso o soporte técnico:

- 📧 **Email:** support@sialitech.com
- 🌐 **Web:** https://sialitech.com
- 📦 **Paquetes:** https://github.com/orgs/Sialitech/packages

---

## 📊 Información Técnica

| Información | Detalle |
|-------------|---------|
| **Versión actual** | 1.0.0 |
| **Total paquetes** | 23 (22 nodos + 1 bundle) |
| **Node-RED compatible** | 2.x - 4.x |
| **Node.js mínimo** | v16+ |
| **Registry** | GitHub Packages |
| **Acceso** | Privado (requiere token) |

---

<div align="center">

**© 2025 Siali Technologies**

RELY Node-RED Nodes - Solución Industrial Completa

</div>
