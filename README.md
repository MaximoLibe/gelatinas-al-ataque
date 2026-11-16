# Gelatinas al Ataque

Tower defense diario en un solo archivo HTML. Cada día hay un mapa nuevo, una regla especial y un grupo de torres disponibles, iguales para todos los jugadores.

## Cómo jugar

Abrí `index.html` en cualquier navegador. No necesita instalar nada.

- Ubicá torres al costado del camino y aguantá 40 rondas de gelatinas.
- Cada gelatina tiene capas: cada golpe le saca una.
- Cada torre elige un **modo de ataque** (3 niveles) y un **potenciador** (2 niveles).
- Árboles, rocas y colinas tapan la visión de las torres. Solo el Francotirador sube a las colinas.
- El Barco solo va en el agua.
- Hay 7 tipos de mapa: Pradera, Barro y hielo, Dos entradas, Túneles, El Ocho, Portales e Islas.

Atajos: teclas 1 a 6 para elegir torre, Espacio para empezar la ronda, F para cambiar la velocidad, Esc para cancelar.

## Notas

- El progreso y las estadísticas se guardan en el navegador.
- Si abrís el archivo directamente desde la compu (sin servidor), el ranking no se conecta.

## Ranking

La versión publicada en GitHub Pages guarda el ranking en Firebase (Firestore) con jugadores anónimos. Las reglas de seguridad están en `firestore.rules`: todos pueden leer el ranking y cada jugador solo puede escribir su propio puntaje.
