# Construcción de RMarkdown con estilo IEEE

## Heramientas necesarias
Para poder compilar y ejecutar sin errores este proyecto, usted debe instalar las siguientes herramientas desde la consola de RStudio.

```r
install.packages(c(
  "rmarkdown",
  "tinytex",
  "xtable",
  "knitr",
  "xfun",
  "pandoc",
  "devtools"
))
tinytex::install_tinytex() # Para fichar la herramienta
update.packages() # Para actualizar todos los paquetes instalados

```

## Configurar el PATH
El programa `pandoc-crossref.exe` debe obligatoriamente agregarlo a las variables de entorno. Para que logre eso siga las siguientes indicaciones.

1. Copia la ruta donde está el programa pandoc-crossref, que debe ser parecida a esto `C:\Users\RSP-L15-LW-001\Documents\IEEEtran-rmarkdown\bin`.
2. Busca `Variables de entorno` y selecciona la primera sugerencia que aparece.
3. Seleccione `Variables de entorno`, luego en `Variables del sistema`, selecciona `Path` y haz clic en `Editar`.
4. Agrega una nueva entrada con la ruta donde está pandoc-crossref.
5. Acepta los cambios y abre una cmd y ejecuta `pandoc-crossref --version`.

