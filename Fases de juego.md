# Fases de juego

La fase de juego corresponden a las dinámicas de juego resueltas por los jugadores. La fase de juego se resuelve dependiendo de las condiciones o lugar de encuentro del jugador, existen tres tipos de fase: (a) fase de exploración, (b) fase de batalla y (c) fase de ciudad.

### (a)	Fases de exploración.

Dicha fase será efectiva si un héroe se encuentra en losetas de bioma.
Cada fase se debe resolver tal como se indica a continuación, de no ser que un evento indique lo contrario, en dicho caso será modificada el psso indicada por el evento y no la totalidad de estos.

1. *Movimientos de héroe*. Cada héroe durante un turno puede utilizar hasta 2 *movimiento de héroe*. Un *movimiento de héroe* permite al héroe moverse un total de 3 + N casillas, donde N es igual al número total de **stats de resistencia**. No es necesario que el héroe se mueva todos los espacios permitidos. Si el jugador termina su movimiento dentro de un poblado o ciudad ir a la (c) **Fase de batalla**. Si termina en una loseta de bioma ir al paso 2.

Una vez se resuelve un movimiento de héroe se sigue al paso 2.

2. *Fase de monstruos*. Esta fase se caracteriza principalmente por la batalla que podría realizar los héroes versus los diversos monstruos.

    2.1.  Antes de comenzar una lucha se debe resolver la cantidad monstruos y su clase. Para esto se lanzaran dos dados: Dado de **cantidad de monstruo** y dado de **clase**, el dado de clase debe ser especifico del bioma en cual se encuentre. Primero se resolverá el dado *cantidad de monstruo*, si este indica cero ir directamente al paso 3, no se lucha. De caso contrario se resolver los dados de *clase*, la clase indica el tipo de monstruo que enfrentara el héroe. Colocar alrededor del héroe el tipo y el número de monstruos (max. número = 3).

    2.1.	Si se los dados son favorables ir al paso 3. De caso contrario ir al paso 2.2.

    2.2.	Para comenzar una lucha el jugador deberá lanzar un dado de monstruo y un dado de cantidad de monstruos. El primero indica que clase de monstruo deberá enfrentar el jugador. El segundo indica en número de monstruos que deberá enfrentar.

    2.3.	Se colocan el/los monstruo(s) al rededor del jugador.

    2.4.	Si existe un héroe a dos casillas de distancia del héroe afectado por esta fase, el héroe afectado podrá solicitar su ayuda y este se incorporará a la batalla solo si este acepta.

    2.5.	Para resolver este paso ver (b) **Fase de batalla**.

3. *Fase de búsqueda*. En esta fase el héroe buscará por los alrededores de su casilla diversos objetos que se podrán escondidos.

    3.1. Un héroe para buscar a su alrededor deberá lanzaran 2 + N **dados de visión**, siendo N igual al número total de **stats de visión**, y un **dado de suerte**. Si el héroe consigue al menos 2 éxitos de visión y la suerte corre a su favor (suerte en dado de suerte) podrá conseguir items dependiendo de sus resultados, considere los siguientes casos:

    *Caso 1*:	Si consigue un número de éxitos igual a un múltiplo de 2, el héroe obtendrá R **items normales**, siendo R igual al residuo de la división entre en número de éxito y 2. Se debe barajar las cartas de *items normales* y se debe sacar un número de cartas igual al residuo.

    *Caso 2*:	Si consigue un número de éxitos igual a un múltiplo de 3, el héroe obtendrá R **items raros**, siendo R igual al residuo de la división entre en número de éxito y 3. Se debe barajar las cartas de *items raros* y se debe sacar sacar un número de cartas igual al residuo.

    *Caso 3*:	Por otro lado, si el número de éxitos lo permite el jugador podrá escoger tanto *items raros* como *items normales*, siguiendo la lógica de los dos casos anteriores. Por ejemplo, si un héroe posee 3 stats de visión deberá lanzar 5 dados de visión más 1 dado de suerte. Si tiene la suficiente suerte, conseguirá 5 éxitos de visión y la suerte estará de su lado (osea que el dado de suerte indica éxito), entonces el héroe podrá decidir si reclama 1 item raro más 1 item normal (usa 5 éxitos de visión) o 2 item normales (usa 4 éxitos de visión).

4. *Fase de contacto*. En este caso el jugador podrá comunicarse con un NPC u otro héroe. Esto solo es cierto si dicho NPC o el héroe se encuentra en una celda adyacente al héroe jugador. De caso contrario ir al paso 5.

    4.1.	Si se comunica con un NPC deberá leer su carta de comunicado, al reverso de la carta NPC y resolver si es así el caso. La información transmitida por el NPC al héroe es secreta y no se deberá revelar a los demás jugadores.

    4.2.	Si se comunica con otro héroe este podrá intercambiar items y/o información. Para el caso de intercambio de items se podrá traspasar cualquier cantidad de items entre los jugadores. En el caso de compartir información, se podrá revelar la información de la comunicación establecida entre los héroes y NPC, para ser así el caso el portador de la información estará en acuerdo de compartir dicha información. Se permite el traspaso de información de terceros y/o mentir.

5. *Fase final*. Si el jugador aun posee movimientos de héroe volver al paso 1, de caso contrario termina su turno y se pasa el turno al siguiente jugador.

### (b)	Fase de batalla

### (c)	Fase de ciudad

Dicha fase será efectiva si un héroe se encuentra en una loseta de pueblo o ciudad.

1. Si el héroe ya se encuentra dentro de la ciudad podrá optar en seguir en la (c) **Fase de ciudad** o ir a la (a) **Fase de exploración**. Si vuelve a la *fase de ciudad* ir al paso 2, de caso contrario ir al paso 1 de la *fase de exploración*.

2. El héroe deberá seleccionar alguna de las siguientes opciones:

  * **Compra de items**: El héroe se puede dirigirse al *mercado de la ciudad* y revisar los items disponibles para comprar, sin embargo, esta información no podrá ser revelado a los demás jugadores. Si el héroe desea comprar un item deberá pagar el precio de compra y mostrar a los demás jugadores la realización de la transacción.

  * **Vender items**: El héroe podrá vender sus items y recibirá su precio en oro por la venta del item.

  * **recuperar vida**: El héroe puede recibir dos **puntos de vida** gratis y podrá comprar *punto de vida* por 10 *monedas de oro* cada uno. EL héroe puede tener hasta un máximo de 5 + N puntos de vida, siendo N el número de **stats de resistencia**.

  * **Comunicación con NPC**: El héroe podrá dirigirse al *Ágora* y leer de cada uno de los NPC de la *sección de pobladores*. El héroe podrá conservar una carta de NPC y resolver dicha *quest* cuando sea necesario. Cada héroe podrá tener hasta un máximo de 3 cartas de NPC y podrá desechar cualquier cantidad de cartas NPC en cualquier fase de su turno.

  * **terminar turno**: Si el héroe desea terminar el turno, pasar al paso 3.

3. Al terminar el turno se debe configurar los siguientes aspectos:

  * Cambiar todos los NPC de la *Ágora* de la ciudad correspondiente y reemplazarlos por 3 NPC nuevos y al azar, todos boca abajo y sin ser revelados.
  * Cambiar 2 items al azar al *mercado de la ciudad* y luego incorporar los items faltantes, todos deben ir boca abajo y sin ser revelados. Deben haber 4 items en el *mercado de la ciudad*.
