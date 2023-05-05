# tic-tac-toe-react-activity
Square: 

Este componente es una representación de un cuadrado del tablero del juego. Recibe como props el valor del cuadrado (X, O o null) y la función onSquareClick que se ejecutará cuando se haga clic en el cuadrado.

Board: 

Este componente es el tablero del juego. Recibe como props xIsNext (un valor booleano que indica si el siguiente movimiento es del jugador X o del jugador O), squares (un arreglo de 9 elementos que representa el estado actual del tablero) y onPlay (una función que se ejecutará cuando se realice un movimiento). Dentro de este componente se define la función handleClick que se ejecutará cuando un cuadrado del tablero sea seleccionado. Esta función verifica si el juego ha terminado, y si no es así, actualiza el arreglo squares con el siguiente movimiento. Luego se llama a la función onPlay para actualizar el estado del juego.

Game: 

Este componente es el componente principal del juego. Contiene el estado del juego (history y currentMove), así como las funciones handlePlay y jumpTo para actualizar el estado del juego. Además, renderiza el tablero del juego y la lista de movimientos en orden cronológico.

CalculateWinner: 

Esta función es una función auxiliar que verifica si un jugador ha ganado el juego. Recibe como parámetro el arreglo squares y verifica si hay tres elementos iguales en una fila, columna o diagonal.
