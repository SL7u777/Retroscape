# RetroScape

PWA para retrospectivas ágiles. En lugar de llenar tarjetas, cada miembro coloca su avatar en un **paisaje compartido** (cima, valle o tormenta) según cómo vivió el sprint, deja **comentarios anónimos por voz o texto**, un **LLM** agrupa los comentarios en temas y propone acciones, y el equipo **vota con fichas** cuáles adoptar como misiones. El paisaje de cada sprint se guarda para ver la evolución del equipo.

Proyecto del curso CC451 Interacción Humano Computadora, Universidad Nacional de Ingeniería, 2026-2.

## Equipo

| Integrante | Caso de uso rediseñado |
|---|---|
| Isaac Antonio Martel Balvin | CU-02 Expresar cómo viví el sprint |
| Diego Alesxander Orrego Torrejon | CU-03 Aportar un comentario anónimo |
| Sebastián Enrique Huaypar Acurio | CU-04 Analizar los comentarios con el LLM |
| Bryan Aldrin Chontay Campos | CU-05 Votar y registrar acciones |

Docente: Ciro Núñez Iturri

## Cómo responde el diseño a los requisitos del curso

| Requisito | Solución |
|---|---|
| Interfaz no convencional | Paisaje con tres zonas en lugar de columnas de tarjetas, con revelación anónima y simultánea |
| Voz | Dictado con transcripción editable y lectura en voz alta de los resúmenes |
| LLM con capa de abstracción | Un servicio intermedio con adaptadores intercambiables (Gemini, OpenAI y uno simulado para pruebas) |
| PWA | Instalable, con manifiesto y service worker; funciona en laptop y celular |
| Personalización continua | Perfil local con preferencias, tiempo de espera del dictado, emociones confirmadas y posición del sprint anterior |
| Multiusuario | Salas con código, sincronización en tiempo real y votación conjunta |
| Diseño emocional (Norman) | Visceral: paisaje, cuenta regresiva y estandartes. Conductual: colocación, dictado y votación con respuesta inmediata. Reflexivo: evolución entre sprints |

## Prototipo navegable

La carpeta `prototipo/` contiene el prototipo de fidelidad media: las 17 pantallas del flujo completo. Para ejecutarlo, en la consola, dentro de la carpeta del repositorio:

```bash
npm start
```

y abre `http://localhost:5173`. Desde ahí también se puede instalar como app (PWA). Los pasos completos están en [docs/instalacion.md](docs/instalacion.md).

## Contenido

```
prototipo/                Prototipo navegable de fidelidad media (PWA)
data/mock/sprints.json    Datos simulados del Equipo Atlas (sprints 11 a 14) para pruebas y demostración
scripts/servidor.js       Servidor local que ejecuta el prototipo (npm start)
docs/
  instalacion.md          Guía de instalación y ejecución
  arquitectura.md         Arquitectura C4 de contexto y contenedores
  requerimientos.md       Requerimientos, historias de usuario y matriz de trazabilidad
  diagramas/              Fuentes PlantUML e imágenes: C4, interacciones y Gantt
  alternativas/           Bocetos de baja fidelidad de las tres alternativas de diseño
```

Otros enlaces:

- [Prototipo en Figma](https://www.figma.com/design/BZ1cMfDsXeL8udWJO67UBA/RetroScape)
- [Diagrama de interacciones entre pantallas](docs/diagramas/interacciones.png)
- [Diagrama de Gantt](docs/diagramas/gantt.png)

## Licencia

[MIT](LICENSE)
