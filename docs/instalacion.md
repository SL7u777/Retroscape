# Guía de instalación

## Requisitos

- Git
- Node.js 18 o superior
- Chrome o Edge

Los comandos de esta guía se escriben en la consola.

## 1. Descargar el repositorio

```bash
git clone https://github.com/SL7u777/Retroscape.git
cd Retroscape
```

El primer comando descarga el repositorio en la carpeta `Retroscape` y el segundo entra en ella.

## 2. Ejecutar el prototipo

Comprueba que Node.js está instalado:

```bash
node -v
```

Debe mostrar `v18` o superior. Luego, dentro de la carpeta `Retroscape`, inicia el prototipo:

```bash
npm start
```

No hace falta `npm install`, porque el proyecto no tiene dependencias. La consola mostrará `Prototipo en http://localhost:5173`.

Abre `http://localhost:5173` en el navegador. Avanza con los botones de cada pantalla, o usa la barra oscura superior para saltar a cualquiera de las 17.

Deja la consola abierta mientras usas el prototipo. Para detenerlo, pulsa `Ctrl + C`.

## 3. Instalarlo como app (PWA)

Con el prototipo abierto en `http://localhost:5173`, pulsa el ícono de instalación en la barra de direcciones. Queda como una app más en el equipo.
