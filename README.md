# Práctica de Git Push y Pull

Repositorio de aprendizaje para practicar la sincronización entre un proyecto local y GitHub mediante `git push` y `git pull`. Incluye archivos de texto con cambios creados localmente y desde el repositorio remoto.

## Contenido

- `archivo1.txt` y `archivo3.txt`: ejemplos de cambios locales para practicar `push`.
- `archivo2.txt` y `archivo5.txt`: ejemplos de archivos creados remotamente para practicar `pull`.
- `archivo4.txt`: ejemplo de trabajo con ramas.
- Historial con un merge y ramas `master` y `nuevaRama`.

## Requisitos

Git y acceso a GitHub. Para subir cambios necesitas permisos de escritura en el repositorio o trabajar sobre tu propio fork.

## Clonar y revisar

```bash
git clone https://github.com/thoonidev/practica-git-push-pull.git
cd practica-git-push-pull
git status
git branch -a
git log --all --oneline --graph --decorate
```

## Subir cambios con push

Modifica `archivo1.txt`, guarda el archivo y ejecuta:

```bash
git add archivo1.txt
git commit -m "Actualiza archivo de práctica"
git push origin master
```

## Recibir cambios con pull

Edita un archivo desde GitHub y confirma el cambio. Después, desde tu copia local y con el trabajo guardado en commits, ejecuta:

```bash
git pull origin master
```

`push` publica tus commits locales; `pull` descarga e integra los cambios remotos en la rama actual. Si ambas copias modificaron las mismas líneas, puede ser necesario resolver un conflicto antes de continuar.

Los archivos son ejemplos de texto: no requieren instalación de dependencias ni un entorno de ejecución.
