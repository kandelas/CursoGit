# repositorio de git y sus fundamentos

son clases del profe herrera
este es un cambio desde el git de visual code
segunda prueba

## carpeta de proton

**<jonathanandrango@protonmail.com>**
2468 contraseña de carpeta

**carpeta compartida**
<https://drive.proton.me/urlsKDME4H4FCG#OUo6y0vw5aTR>


###### git es un controlador de versiones, quiere decir que puede almacenar o registrar los cambios realizados a través del tiempo.
##### Versión
```bash
git --version
```
##### Ayuda
```bash
git --help
git --help add
```
---
## Configuración.
### Usuario
```bash
git --config --global user.name "Kan"
```
### Email
```bash
git config --global user.email "Kan@gmail.com"
```
### Archivo Configuración
```bash
git config --global -e
```
### Configuración de Rama por Defecto
```bash
git config --global init.defaultBranch "main"
```

## Iniciar un Repositorio de Git
### Añadir todo al Stage
```bash
git init
```
---
## Stage  
### Añadir todo al Stage
```bash
git add .
```
### Añadir al Stage con Extensión
####  comodines
- ###### Archivos con extensión    **.html**
```bash
git add *.html
```
- ###### Archivos con extensión    **.css**
```bash
git add *.css
```
- ###### Archivos con extensión especificando el directorio donde se encuentran    **.js**
```bash
git add js/*.js
```
- ###### Todos los archivos que  se encuentran en dicha dirección    **/**
```bash
git add style/
```

### Añadir uno a uno los archivos al Stage
```bash
git add nombreArchivo
```
### Remover un archivo del  Stage
```bash
git reset nombreArchivo
```

---
## Commit
###  Hacer un commit con un mensaje 
```bash
git commit -m  " mi primer commit "
```
######  Subiendo al stage y haciendo el commit al mismo tiempo 
```bash
git commit -am  " mi primer commit "
```
###  Hacer una corrección el  mensaje del    commit
```bash
git commit --amend -m " mi primer commit corregido"
```
### Reconstruir desde el ultimo commit
###### Reconstruir todo desde el ultimo commit o foto
```bash
git checkout -- .
```
### Remover Commit
###### Remover todo el commit
```bash
git reset --soft idCommitParaResetear
```
###### Remover  el commit desde el HEAD
```bash
git reset --soft HEAD^idCommitParaResetear
```
---
## Alias
###### Alias [s] para status
```bash
git config --global alias.s status
```
###### Alias [a] para agregar todo al stage
```bash
git config --global alias.a 'add .'
```
###### Alias [c] para config --global
```bash
git config --global alias.c 'config --global'
```
###### Alias [lg] para log
```bash
git config --global alias.l log
```
###### Alias [l] para un  log sofisticado
```bash
git config --global alias.l "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(yellow bold)%d%C(reset)' --all"
```

