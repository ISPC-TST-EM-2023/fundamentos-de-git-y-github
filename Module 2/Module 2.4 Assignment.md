# Módulo 2.4 Tarea

En esta lección, aprendió acerca de los conflictos de combinación. Para completar esta tarea, creará un archivo `README.md` que dice "Hello World". Copie y pegue los siguientes comandos en su línea de comando, luego presione Entrar:

```
mkdir MergeConflict
cd MergeConflict/
git init
touch README.md
echo "echo Hello" > README.md
git add .
git commit -m "first commit on master"
git checkout -b new-branch
echo "Hello World" > README.md
git add .
git commit -m "first commit on new-branch"
git checkout master
echo "Hola" > README.md
git add .
git commit -m "second commit on master"
git merge new-branch
```

Este "script" creará un conflicto de combinación. Resuelva el conflicto de combinación para que el texto en `README.md` sea `"Hello World"`.

## Envío
Para enviar esta tarea, cree un problema titulado "Asignación del módulo 2.4" en este repositorio. En el problema, proporcione una captura de pantalla de su línea de comando que muestre los comandos que usó para resolver el conflicto de combinación en esta tarea, luego continúe con el siguiente módulo.
