# Control de versiones con Git y GitHub

## 1: Configuración de Git
Ejecutar la consola de Git (Git Bash) y establecer el nombre del usuario y el correo (vinculado a GitHub).

```Git
git config --global user.name "Nombre o Usuario"
git config --global user.email "correo@gmail.com"
```

## 2: Iniciar repositorio
En el directorio del proyecto abrir la consola de Git Bash o un nuevo terminal (en caso de Visual Studio Code).

Iniciar el repositorio.
```Git
git init
```

## 3: Crear un archivo README.md
Crear un archivo Markdown *README.md* para la documentación del proyecto que contenga como título "# Proyecto X".
```Git
echo "# Proyecto X" > README.md
```

## 4: Agregar archivos al área de preparación
Agregar uno o varios archivos específicos
```Git
git add README.md
```

Agregar todos los archivos (nuevos, modificados, eliminados).
```Git
git add .
```
o
```Git
git add -A
```

Agregar solo archivos modificados y eliminados (actualización de cambios).
```Git
git add -u
```

## 5: Commit de los cambios
Se guarda los cambios incluyendo un mensaje descriptivo.
```Git
git commit -m "Agrega archivo README.md y X archivos"
```

## 6: Retirar un archivo del área de preparación
Se crea un archivo y se agrega al área de preparación.
```Git
git echo "Recordatorio ..." > Nota.txt
git add Nota.txt
```

Se retira del área de preparación.
```Git
git reset
```

## 7: Ver estado actual del repositorio
```Git
git status
```

## 8: Crear un Repositorio en GitHub
* Entra a GitHub y accede a tu cuenta.
* Haz clic en "New repository" (Nuevo repositorio).
* Ponle un nombre a tu repositorio.
* Elige "Public" o "Private" según prefieras.
* No marques "Initialize this repository with a README" (esto es importante si ya tienes archivos en tu computadora).
* Haz clic en "Create repository".

## 9: Conectar tu repositorio local con GitHub
En la terminal, ejecuta este comando para vincular el repositorio remoto.
```Git
git remote add origin https://github.com/tu-usuario/nombre-del-repositorio.git
```

## 10: Sube los cambios al repositorio remoto en GitHub
La rama master del repositorio local se renombra por main
```Git
git branch -M main
```

Se envía los cambios a GitHub
```Git
git push -u origin main
```
