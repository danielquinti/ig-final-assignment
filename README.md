# Presentación NIC — Neural Image Compression

## Requisitos

Se necesita una instalación de TeX Live con los siguientes paquetes:

- `beamertheme-metropolis` (tema Beamer Metropolis)
- `pgfopts` (dependencia de metropolis)

## Instalación de dependencias

```bash
# macOS / Linux (requiere permisos de administrador)
sudo tlmgr install beamertheme-metropolis pgfopts
```

Si no tienes permisos de administrador, puedes instalar en modo usuario:

```bash
tlmgr init-usertree
tlmgr --usermode install beamertheme-metropolis pgfopts
```

## Compilación

```bash
pdflatex main.tex
pdflatex main.tex   # segunda pasada para índice correcto
```

## Limpiar archivos temporales

```bash
rm -f *.aux *.log *.nav *.snm *.toc *.out contents/*.aux
```

## Imágenes

Las figuras están comentadas en los archivos `contents/*.tex`. Para activarlas, descomenta los bloques `\begin{figure}...\end{figure}` y coloca las imágenes correspondientes en `images/`:

- `images/vae_architecture.png`
- `images/evolucion_arquitecturas.png`
- `images/curva_rd.png`
- `images/comparacion_perceptual.png`
