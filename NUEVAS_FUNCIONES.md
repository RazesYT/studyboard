# 📚 StudyBoard - Nuevas Funcionalidades

## 🎨 Export PDF Profesional

### ¿Cómo usar?
1. En la vista de asignaturas, haz clic en el menú FAB (botón flotante ✨)
2. Selecciona el botón 📄 "Exportar PDF"
3. Personaliza tu informe:
   - ✅ Portada con título y fecha
   - ✅ Estadísticas generales (promedio, aprobadas, ECTS)
   - ✅ Gráficos de distribución de notas
   - ✅ Detalle completo por asignatura
   - ✅ Recomendaciones de la IA
4. Edita el título del informe (ej: "Informe Académico Q1 2025")
5. Haz clic en "Generar PDF"

### Características del PDF:
- 📊 **Diseño profesional** con colores corporativos
- 📈 **Estadísticas visuales** de tu rendimiento
- 📚 **Detalle por asignatura** con notas y progreso
- 🤖 **Recomendaciones personalizadas** basadas en IA
- 📄 **Múltiples páginas** con numeración automática
- 💾 **Descarga instantánea** sin necesidad de internet

### Casos de uso:
- Mostrar progreso a padres/tutores
- Guardar registro de cada cuatrimestre
- Adjuntar a solicitudes académicas
- Compartir con profesores/orientadores

---

## 📱 Widget para Móviles

### ¿Qué es?
Un widget independiente que muestra tus estadísticas en tiempo real sin abrir la app completa.

### ¿Cómo acceder?
**Opción 1: Acceso directo**
- Abre `widget.html` directamente en el navegador
- Guarda como favorito en tu pantalla de inicio

**Opción 2: Desde el menú de la PWA** (iOS/Android)
1. Instala StudyBoard como PWA
2. Mantén presionado el icono de la app
3. Selecciona "Widget Información" en los atajos

**Opción 3: Marcador en pantalla de inicio**
1. Abre `widget.html` en Safari/Chrome
2. Menú → "Añadir a pantalla de inicio"
3. Personaliza el nombre (ej: "📊 StudyBoard")

### Información mostrada:
- 📊 **Promedio general** con emoji dinámico
- 📚 **Total de asignaturas** activas
- ✅ **Asignaturas aprobadas**
- 🎓 **ECTS acumulados**
- ⏰ **Última actualización**

### Características:
- 🎨 **Diseño elegante** con gradiente animado
- 🔄 **Actualización automática** cada minuto
- 📱 **Responsive** para todos los tamaños
- ⚡ **Ultra rápido** sin cargar la app completa
- 💾 **Datos en tiempo real** desde localStorage

### Tamaños disponibles:
- 📱 **Widget pequeño** (iOS): Solo promedio y asignaturas
- 📊 **Widget mediano**: Todas las estadísticas
- 📈 **Widget grande**: Stats + acceso directo

---

## 🚀 Próximas mejoras

### Export PDF v2.0:
- [ ] Gráficos visuales (canvas/charts)
- [ ] Comparativa entre cuatrimestres
- [ ] Exportar a Excel
- [ ] Enviar por email directo
- [ ] Modo claro/oscuro en PDF

### Widget v2.0:
- [ ] Próximo examen con cuenta regresiva
- [ ] Configuración de tamaño
- [ ] Múltiples temas/colores
- [ ] Widget interactivo (añadir notas)
- [ ] Notificaciones push

---

## 📖 Documentación técnica

### Export PDF
**Biblioteca utilizada:** jsPDF v2.5.1  
**CDN:** https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js  
**Carga:** Dinámica (solo cuando se usa)  

**Estructura del PDF:**
1. Portada (página 1)
2. Estadísticas generales
3. Distribución de notas
4. Detalle por asignatura (múltiples páginas)
5. Recomendaciones IA
6. Pie de página en todas las páginas

### Widget
**Archivo:** `widget.html`  
**Dependencias:** Ninguna (vanilla JS)  
**Datos:** Lee desde `localStorage` (sincronizado con app principal)  
**Actualización:** Cada 60 segundos + al obtener foco  

**Compatibilidad:**
- ✅ iOS Safari (Home Screen Web App)
- ✅ Android Chrome (PWA Shortcut)
- ✅ Desktop (cualquier navegador)

---

## 💡 Tips

### Para mejor experiencia en móvil:
1. Instala la PWA completa
2. Añade el widget a pantalla de inicio
3. Usa ambos según necesites:
   - Widget: Vista rápida
   - App: Gestión completa

### Para generar PDFs perfectos:
1. Actualiza todas tus notas antes
2. Verifica el progreso evaluado
3. Revisa las recomendaciones IA
4. Personaliza el título del informe
5. Desmarca lo que no necesites

---

## 🐛 Solución de problemas

**El PDF no se descarga:**
- Verifica que tu navegador permite descargas
- Prueba en modo incógnito
- Comprueba que hay datos para exportar

**El widget no muestra datos:**
- Asegúrate de tener asignaturas creadas
- Verifica que el widget.html está en la misma carpeta
- Recarga la página (F5)

**Widget no actualiza:**
- Cambia a la app principal y vuelve al widget
- Cierra y vuelve a abrir
- Limpia caché del navegador

---

## 📞 Soporte

¿Problemas o sugerencias?  
Abre un issue en: https://github.com/RazesYT/studyboard

---

**Versión:** 2.0.0  
**Fecha:** Noviembre 2025  
**Autor:** RazesYT
