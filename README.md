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

Hacemos el commit D en la rama exp despues de escribir en main
```bash
git commit -a -m "D"
```