## 👥 Integrantes del Equipo
- **Alejandro Galindo**
- **Daniel Luque** 
- **Andres Mancera** 

---

# Comandos Básicos de Git y GitHub ​🤯

# Que es Git Hub 👀​

GitHub es una plataforma en línea que sirve para guardar, compartir y trabajar en proyectos de programación usando Git (el sistema de control de versiones).

## Con GitHub puedes:

- Guardar tu código en la nube (repositorios).

- Trabajar en equipo: varios programadores pueden colaborar en el mismo proyecto.

- Llevar historial de cambios (commits).

- Crear ramas (branches) para probar nuevas funciones sin dañar el proyecto principal.

- Subir y bajar proyectos desde cualquier lugar.

- Conectar tu proyecto con herramientas de despliegue, automatización y pruebas.

## 📌 Ejemplo sencillo:

- Git = es la herramienta que controla versiones en tu PC.

- GitHub = es el sitio web donde subes esos proyectos para colaborar y compartir.

## 🔧 Comandos Esenciales de Git y GitHub

### Configuración Inicial y Clonado
```bash
# Configurar usuario
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@ejemplo.com"

# Clonar repositorio del equipo
git clone https://github.com/usuario/repositorio.git
cd repositorio
```

### Flujo de Trabajo Básico
```bash
# 1. Actualizar repositorio local
git pull origin main

# 2. Ver estado de archivos
git status

# 3. Agregar cambios al staging
git add .                         # Todos los archivos
git add nombre-archivo.txt        # Archivo específico

# 4. Hacer commit
git commit -m "Descripción clara del cambio"

# 5. Subir cambios al repositorio remoto
git push origin main
```

### Trabajo con Ramas (Recomendado para el equipo)
```bash
# Crear y cambiar a nueva rama personal
git checkout -b feature/tu-nombre

# Hacer cambios, add y commit
git add .
git commit -m "Agregar contribución de [Tu Nombre]"

# Subir rama al repositorio remoto
git push origin feature/tu-nombre

# Volver a rama principal y actualizar
git checkout main
git pull origin main
```

### Comandos de Información y Control
```bash
# Ver historial de commits
git log --oneline

# Ver diferencias
git diff

# Ver ramas
git branch -a

# Deshacer cambios no guardados
git checkout -- nombre-archivo.txt

# Ver repositorios remotos
git remote -v
```


## 🚨 Comandos de Emergencia

```bash
# Si hay conflictos al hacer pull
git stash                         # Guardar cambios temporalmente
git pull origin main             # Actualizar
git stash pop                     # Restaurar cambios

# Si necesitas deshacer el último commit
git reset --soft HEAD~1          # Mantiene los cambios
git reset --hard HEAD~1          # Elimina los cambios

# Si tu rama se desincronizó
git fetch origin
git reset --hard origin/main
```

---

## ✏️ Gracias por ver 