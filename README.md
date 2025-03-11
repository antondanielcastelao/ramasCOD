# Ramas y merge en github

Vamos a hacer el commit "A"
```bash
git commit -a -m "A"
```
Ahora el commit "B"
```bash
git commit -a -m "B"
```

## Creación de una rama
Visualizamos nuestras ramas, en la que trabajemos saldra marcada con un asterisco.
```bash
git branch
```

Para crear una rama usamos el argumento brach
```bash
git branch exp
```

Cambiamos a esa rama con checkout
```bash
git checkout exp
```

Ahora hacemos el commit C en la rama exp
```bash
git commit -a -m "C"
```
Podemos seguir haciendo commits paralelamente a la rama main sin afectar exp si hacemos checkout
```bash
git checkout main
git commit -a -m "E"
```

Hacemos el commit D en la rama exp despues de escribir en main
```bash
git checkout exp
git commit -a -m "D"
```

## Union mediante merge
Finalmente unimos las dos ramas usando el comando merge. Vamos a la rama main y mergeamos con exp.
```bash
git checkout main
git merge exp
```
Puede que de algunos errores si los archivos entran en conflicto pero el IDE tiene un asistente con el cual hacer los cambios oportunos teniendo en cuenta la rama origen como la que va a ser mergeada.