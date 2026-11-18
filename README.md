# Gelatinas al Ataque

Tower defense diario en un solo archivo HTML. Cada día hay un mapa nuevo, una regla especial y un grupo de torres disponibles, iguales para todos los jugadores.

## Cómo jugar

Abrí `index.html` en cualquier navegador. No necesita instalar nada.

- Ubicá torres al costado del camino y aguantá 40 rondas de gelatinas.
- Cada gelatina tiene capas: cada golpe le saca una.
- Cada torre elige un **modo de ataque** (3 niveles) y un **potenciador** (2 niveles).
- Árboles, rocas y colinas tapan la visión de las torres. Solo el Francotirador sube a las colinas.
- El Barco solo va en el agua.
- Hay 10 tipos de mapa: Camino largo, Barro y hielo, Dos entradas, Túneles, El Ocho, Portales, Islas, Cruce, Río y puente, y Espiral.

Atajos: teclas 1 a 5 para elegir torre, Espacio para empezar la ronda, F para cambiar la velocidad, Esc para cancelar.

## Novedades desde el 19/11/2026

Los mapas de antes de esa fecha se generan igual que siempre, así sus rankings siguen valiendo. Desde el 19/11:

- **Mapas nuevos:** Cruce (dos caminos que se cruzan), Río y puente (el Barco navega el río) y Espiral (termina en el centro).
- **Ambientes:** pradera, desierto (tormentas de arena que achican el alcance), nieve (más rápidas, pero el hielo dura más), volcán (lagos de lava y erupciones) y noche (se ve menos sin un Faro).
- **Torres nuevas:** Rayo (salta de gelatina en gelatina), Faro (mejora a las torres de alrededor) y Granja (da plata al terminar cada ronda). Cada día hay 5 de las 9.
- **Gelatinas nuevas:** Cometa (rapidísima), Voladora (vuela derecho, sin seguir el camino) y Curandera (devuelve capas a las de alrededor).
- **Eventos:** algunas rondas traen un caso especial: Fiebre del oro, Estampida, Niebla espesa, Lluvia de burbujas, Viento en contra o Lluvia de meteoros.
- **Tecnologías:** antes de la ronda 1 y después de las rondas 10, 20 y 30 se elige una mejora para toda la partida.
- **Reglas nuevas:** Inflación, Bandada, Hospital y descuentos para las torres nuevas.

## Notas

- El progreso y las estadísticas se guardan en el navegador.
- Si abrís el archivo directamente desde la compu (sin servidor), el ranking no se conecta.

## Ranking

La versión publicada en GitHub Pages guarda el ranking en Firebase (Firestore) con jugadores anónimos. Las reglas de seguridad están en `firestore.rules`: todos pueden leer el ranking y cada jugador solo puede escribir su propio puntaje.
