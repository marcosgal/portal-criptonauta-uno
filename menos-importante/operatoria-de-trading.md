# Operatoria de trading

#### NOT-A-DISCLAIMER = ERES RESPONSABLE DE TU DINERO!

#### El riesgo al operar en criptomonedas con apalancamiento es muy alto. Y eres 100% responsable de tus decisiones financieras.

El autor de este libro no aceptará ninguna responsabilidad respecto de las decisiones tomadas por terceros.

&#x20;

A esta altura **solo deberías continuar leyendo** si estás registrado en la testnet de Bitmex, aprendiste a utilizar sus tipos de órdenes leyendo [el manual](https://www.bitmex.com/app/tradingOverview) que la plataforma brinda para todos sus usuarios, y analizaste gráficos de acuerdo a lo expuesto en los capítulos anteriores.

Si aún no lo hiciste, **ES NECESARIO** que comiences a practicar y continúes luego de haberte familiarizado con las criptomonedas y el _exchange_ donde vas a abrir tus posiciones.

&#x20;

En caso de que ya estés preparado para avanzar, continuamos.

&#x20;

Evitar errores en el manejo de la plataforma es igual de importante que mantener constancia respecto de una estrategia de _trading_, por lo que nuevamente te aconsejo [leer el manual que brinda BitMex](https://www.bitmex.com/app/tradingOverview) y además prestar especial atención a este capítulo.

Todas las pruebas en la plataforma **LAS TENÉS QUE REALIZAR EN LA PLATAFORMA DEMO**.

&#x20;

Aprendí a los golpes. SIEMPRE hay tiempo para hacer dinero. Tenés que familiarizarte con el exchange y nada mejor que lo hagas de manera relajada y sin presiones.

## La interfaz gráfica

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Interfaz completa de Bitmex en testnet.</p></figcaption></figure>

1. Panel para ejecutar órdenes (compras, ventas, _stop-loss_, _take profit_).
2. Selector de _leverage_ (apalancamiento).
3. Libro de órdenes (se puede extender _clickeando_ sobre el ícono del medio en su extremo superior derecho).
4. Gráfico con las órdenes en tiempo real.
5. Posiciones tomadas (abiertas, activas, cerradas, stop-loss, órdenes parcialmente llenas e historial completo).
6. Información acerca del activo elegido para operar.

## CALCULADORA: ROE, LIQUIDACIÓN

Antes de realizar cualquier movimiento en la plataforma, es indispensable que utilices la calculadora que el sitio incorpora _clickeando_ en el ícono de la parte superior izquierda del _exchange_, tal como se ve en la siguiente imagen:

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption><p>Calculadora en Bitmex</p></figcaption></figure>

A partir de esta herramienta vas a poder calcular:

\- **Eventuales ganancias:** fijando el _take profit_ en _exit price_ en la primera pestaña (Profit/Loss). Se visualiza como ROE.

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption><p>Calculadora en Bitmex (take profit en exit price). Futuros de TRX en testnet.</p></figcaption></figure>

&#x20;\- **Porcentaje de pérdida:** fijando el valor exacto del _stop-loss_ en _exit price_.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption><p>Calculadora en Bitmex (SL como exit price). Futuros de TRX en testnet.</p></figcaption></figure>

El **ROE** es el cálculo del retorno de una posición con comisiones incluidas. Como mencioné anteriormente, puede calcular eventuales ganancias (fijando el _take-profit_ en _“exit price”_) así como también pérdidas (fijando el _stop-loss_ en _“exit price”_).

&#x20;

**NOTA:** en “Leverage” deberías fijar el apalancamiento que deseés utilizar.

&#x20;

\- **Precio de liquidación:** voy a desarrollar esto más adelante, dada su relevancia. Como regla general, tu _stop-loss_ NUNCA debería superar (en operaciones a _short_) o estar por debajo (en operaciones a _long_) el valor de liquidación porque eso equivaldría a la pérdida de la posición y que el _stop-loss_ no se ejecute.

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption><p>Cálculo de precio de liquidación (Futuros de TRX en testnet).</p></figcaption></figure>

Es importante que prestes atención al interruptor que permite calcular posiciones a _long_/_short_ porque de lo contrario el cálculo te va a devolver valores invertidos (las pérdidas se mostrarían en números positivos mientras que las ganancias en números negativos).

&#x20;

Una vez que hayas definido la estrategia en la herramienta de análisis de gráficos y luego de calcular eventuales ganancias (_take profit_), porcentaje de pérdidas tolerado (_stop-loss_) y precio de liquidación (_liquidation price_), tenés que fijar las órdenes en Bitmex. Te aconsejo empezar por los _stop-loss_.

## FIJAR CORRECTAMENTE LOS STOP-LOSS

En Bitmex es **IMPORTANTE** que utilices DOS _stop-loss_: uno de tipo _limit_ y otro de tipo _market_. Esto tiene la finalidad de proteger tu posición ante eventuales pérdidas de dinero, recordá que al trabajar con margen el _exchange_ puede liquidar tu posición (dejarla en cero) en caso de que el mercado no responda de la manera esperada.

&#x20;

Las órdenes _stop-limit_ pueden fijarse con el mismo valor (esto le daría la orden al _exchange_ de que, si el precio llega al valor X, las órdenes de compra/venta se coloquen a ese mismo valor), o bien con una pequeña diferencia, para asegurar que las mismas se ejecuten al valor Y.

En el caso de que estés en una posición _long_, el _stop-limit_ deberá ser una orden de venta y deberías fijar el _stop price_ apenas por debajo del _limit price_ al que vas a colocar la orden.

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption><p>Stop-loss de tipo limit en una operación a long.</p></figcaption></figure>

En sentido contrario, en una posición a _short_, el _stop-limit_ debería ser una orden de compra y el _stop price_ debería estar apenas por encima del _limit price_.

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption><p><em>Stop-loss</em> de tipo <em>limit</em> en una operación a <em>short</em>.</p></figcaption></figure>

La finalidad de fijar una variación mínima de precio entre el _stop price_ y el _limit price_, es cubrir la posición ante fluctuaciones fuertes de mercado.

Si las órdenes de compra/venta se ejecutan con mucha fuerza, puede que la orden _limit_ que definiste en tu _stop-loss_ se abra, pero el precio haya superado ese valor y no se pueda ejecutar. Esto generaría pérdidas innecesarias y, en el peor de los casos, la liquidación de tus posiciones.

&#x20;

En Bitmex, como recomendé antes, deberías además fijar un _stop-loss_ de tipo _market_ para asegurar aún más tu posición. Tené en cuenta que los _stop-loss_ no implican gastos de ningún tipo, solo lleva unos segundos fijarlos.

En la siguiente imagen podés ver un _stop-loss_ a precio _market_ que complementa el de tipo _limit_ fijado anteriormente.

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption><p>SL de tipo market (click en la flecha para seleccionar).</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption><p>Orden abierta a short con stop loss limit y market (futuros de ADA en testnet).</p></figcaption></figure>

## INGRESAR POSICIÓN EN BITMEX

Una vez fijados los _stops_, tenés que ingresar la posición a partir una orden de compra/venta _limit_ o _market_:

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption><p>Ingresar órdenes limit (reciben comisión).</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption><p>Ingresar órdenes market (pagan comisión).</p></figcaption></figure>

La casilla _“Post-Only”_ en las órdenes de tipo _limit_ establecen que la orden no se ejecute si el valor fijado en la misma se ejecutaría a valor del mercado (porque coinciden). Te recomiendo mantenerla tildada así evitás que te cobren comisión desde órdenes que deberían recibirla.

## PNL: PROFIT AND LOSS

Una vez abierta una operación, la misma figura en la parte inferior de la plataforma junto a un indicador denominado PNL (_“profit and loss”_).

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption><p>Profit and loss en Bitmex.</p></figcaption></figure>

**Unrealised PNL:** retorno (ROE) de la operación a [mark price](https://www.bitmex.com/app/fairPriceMarking) sin tener en cuenta la comisión de salida.

**Realised PNL:** tomas de ganancias o pérdidas parciales, si cerraste solo algunos contratos de la operación inicial.

&#x20;

Al posicionar el mouse sobre el _Unrealised PNL_, podés ver el PNL (retorno) final sumando una orden de salida de tipo _market_ al [mark price](https://www.bitmex.com/app/faq):

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption><p>Unrealised PNL final</p></figcaption></figure>

## TOMA DE GANANCIAS EN BITMEX

La toma de ganancias, tal como comenté en el capítulo anterior, dependerá de tu personalidad. Por mi parte generalmente cierro las operaciones cuando el precio se acerca al cruce de medias móviles, o cuando visualizo una vela que indique reversión. Si estoy conforme con el 5% o 10% del trade, salgo y aseguro el _profit_.

El _order book_ puede definir el momento exacto de la salida si muestra una fuerte presión a la inversa de mi posición.

&#x20;

Pienso que deberías intentar órdenes _limit_ al momento de tomar ganancias, salvo que el mercado muestre señales de alta volatilidad. En tal situación, una orden _market_ puede cerrar la posición instantáneamente por un coste mínimo de comisión. Siempre es preferible que asegures _profits_ antes que perder dinero.

Es muy importante que entiendas que solo estás fuera del mercado si la posición se completó. Que el precio llegue al valor de una orden _limit_, no asegura que la misma se ejecute.

&#x20;

Tené presente que si fijás tus órdenes de tipo _limit_ uno o dos _satoshis_ por debajo del precio con mayor cantidad de órdenes activas, es más probable que las mismas se ejecuten.

&#x20;

Al trabajar haciendo _scalping_, los movimientos suelen darse muy rápido por lo que en general ingreso la posición inicial ejecutando una orden de tipo _market_ (para no perder la entrada) y luego cierro -en la medida de lo posible, de acuerdo con la liquidez y situación del mercado- con una orden de tipo _limit_, para recibir el pago de la comisión y aumentar los beneficios.

## TRAILING STOP

Otra manera de tomar ganancias en Bitmex se puede realizar a partir de _trailing stops_. Con este tipo de órdenes podés maximizar beneficios determinando un _stop-loss_ que se mueve a medida que el precio avanza.

Para fijarlo tenés que elegir la opción desde el menú y definir la diferencia que querés que mantenga el SL:

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption><p>(Trailing stop en la testnet de Bitmex)</p></figcaption></figure>

**En LONG**: supongamos que fijás tu _trailing stop_ a -50 dólares de diferencia en un precio de $9000. El precio de BTC continúa al alza hasta los $9300 pero luego se devuelve. Tu SL se ejecutaría a los $9250.

**En SHORT**: ahora suponemos que fijás tu _trailing stop_ a 50 dólares (en positivo) de diferencia cuando el precio toca los $8000. Si BTC genera _profit_ hasta los 7800 pero luego se devuelve al alza, tu SL se ejecutaría a los $7850.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption><p>(Diferencia que mantiene el trailing stop)</p></figcaption></figure>

Tené en cuenta que la orden en este caso se ejecutaría como _taker_, por lo que pagaría comisión y tenés que fijar estas órdenes con una previamente abierta (posición _a long_ o _a short_).

Personalmente prefiero cerrar las posiciones por mi cuenta, pero es una opción interesante si querés dejar correr ganancias ante una eventual ruptura de lateralidad o canal tendencial a favor de tu posición.

## ¿CÓMO EVITAR “LIQUIDACIONES”?

Como anticipé varias veces, Bitmex incorpora un sistema de _liquidaciones_ que, en términos prácticos, permite que el exchange se _cobre_ las pérdidas no administradas correctamente. Miles de operadores pierden sus posiciones e incluso todo su capital y es prácticamente desde donde sus creadores y quienes gestionan la plataforma, obtienen dinero.

Esto sucede, en primer lugar, por ignorancia por parte de _traders_ novatos y, en segundo lugar, porque _traders_ experimentados no ahondan en los distintos tipos de órdenes de la plataforma y a base de prueba y error, entienden (o no) de qué manera pueden cubrir sus posiciones y asegurar sus pérdidas.

&#x20;

Bitmex, al igual que cualquier empresa, obtiene beneficios por prestar su servicio; el mercado no regulado de las criptomonedas puede ser manipulado desde la misma plataforma en vista de liquidar posiciones, sobre todo las apalancadas a 50X y 100X que tienen un margen de acción realmente estrecho.

En el siguiente gráfico se pueden ver picos que XBT realiza diariamente, tanto al alza como a la baja. La intención de este tipo de movimientos es liquidar a quienes abren posiciones con un _leverage_ mayor a 20X sin fijar _stop-loss_ o fijándolos de manera incorrecta.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption><p>Liquidaciones de long y shorts en Bitmex</p></figcaption></figure>

Existen ciertos detalles que pueden determinar o no la liquidación de una posición. Aprendí esto que voy a comentar exclusivamente desde mi experiencia porque no suele ser algo que la mayoría de los traders decida comentar. Tal vez por vergüenza, tal vez porque desean que el resto aprenda _“a los golpazos”_. Valoraría mucho que lo tengas presente.

&#x20;

#### Operar alternativas a XBT, ETH y LTC

&#x20;

XBT, ETH y LTC son las monedas con mayor volatilidad -que se ve justamente incrementada por liquidaciones-. Los pares restantes de _criptos_ aceptados por la plataforma, son por definición menos riesgosas.

La volatilidad aumenta exponencialmente en mercados en crecimiento y que permitan además apalancamientos tan elevados como 50/100X. Te aconsejo probar las ALTs (tené en cuenta que siempre ganás XBT).

&#x20;

#### Operar períodos tendenciales o canales de tendencia

&#x20;

En períodos laterales se puede trabajar de manera mucho más tranquila que buscando _breakouts_. Al menos te aconsejo que pruebes la idea de operar en ese momento, es probable que puedas adaptar mi estrategia a velas de 1H o 4H si no te animás a hacer _scalping_.

&#x20;

#### Comenzar operando con leverage MENOR a 10x

&#x20;

Es fundamental que respetes esta premisa, al menos hasta que te sientas cómodo con la plataforma y tus resultados en la _testnet_ o con capital simbólico, sean mayormente positivos y consistentes.

Si nunca trabajaste con margen, 2X o 3X son suficientes para obtener buenos retornos. Recordá siempre que lo importante al momento de hacer _trading_ es la consistencia.

&#x20;

#### **Fijar** stop-loss **de tipo** limit **en combinación con una órden de tipo** market

&#x20;

Este _tip_ es clave para proteger posiciones y asegurar que el _stop-loss_ se ejecute. En los párrafos anteriores te comenté paso a paso de qué manera hacerlo, pero lo menciono nuevamente para que estés atento de su importancia.

&#x20;

#### **Fijar el** stop-loss **de tipo** market **utilizando el** “mark price”

&#x20;

El manual de Bitmex ofrece una explicación muy clara de las diferencias entre _last price_ y _mark price_ al momento de fijar los _stop-loss_.

En general una orden _market_ fijada en _last price_ suele ser suficiente, pero si querés asegurar al máximo tus posiciones, deberías prestar atención a este párrafo y probar en la _testnet_ el _stop-loss_ fijado a _“mark price”_. Este último tiene la contra de que puede cerrar una posición antes de tiempo, pero asegura la pérdida frente a una fluctuación muy fuerte del mercado.

&#x20;

#### Evitar ingresar a una posición en Bitmex luego de una vela que represente dos o tres veces el volumen de la vela anterior

&#x20;

Esto indica volatilidad y es probable que anticipe un cambio o continuación de tendencia (alcista o bajista). El libro de órdenes en estos momentos manifiesta picos y variaciones realmente muy pronunciados y es realmente muy riesgoso operar en esos momentos. Para muchos/as puede ser algo excitante, pero desde mi humilde opinión, no es hacer _trading_.

&#x20;

#### Evitar perseguir una vela

&#x20;

Si al momento en el que estás operando comenzás a ver que las órdenes _market_ comienzan a arrasar con las órdenes _limit_, te aconsejo mantenerte lo más lejos que puedas del mercado.

La volatilidad cuando se abandona la zona lateral o el canal tendencial, suele ser muy fuerte y es realmente muy difícil poder ingresar con criterio y mucho menos apalancando. El precio en estas situaciones suele moverse en ambas direcciones hasta consolidarse, por lo que pienso que hay mejores momentos para operar.

Las pérdidas que podés tener intentando perseguir una vela de gran cuerpo, ya sea alcista o bajista, son realmente muy grandes. Te aconsejo mantenerte lejos.

## ¿SYSTEM OVERLOADED?

&#x20;

Bitmex tiene una contra muy grande frente a otros exchanges y considero estrictamente necesario brindarle un espacio a ella en este libro. Es probable que si pretendés mover tus órdenes (entradas o _stop-loss_ de tipo _limit_) te encuentres con el siguiente mensaje en más de una ocasión:

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption><p>“Order Submission Error”, el fantasma de Bitmex.</p></figcaption></figure>

Por este motivo en su momento intenté buscar una alternativa al _exchange_, que acepte _leverage_ en criptomonedas y las mismas órdenes que ofrece Bitmex (compras y _stops market/limit_, _trailing stop_) pero hasta el momento ninguna ofrece liquidez aceptable sin KYC y por ese motivo elaboré una manera de operar en la plataforma sin tener problemas con esta situación.

&#x20;

Bitmex [explica en su web](https://www.bitmex.com/app/loadShedding) que las órdenes se ubican en una cola de procesamiento, y son ejecutadas de acuerdo al orden en el que llegan a la misma.

En momentos de mucha demanda -usualmente durante los _breakouts_- las órdenes que ingresan al sistema de procesamiento exceden su capacidad por lo que, en esa situación, el sistema las rebota.

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption><p>Procesamiento de órdenes (Bitmex). La última posición en ingresar es rebotada.</p></figcaption></figure>

¿Qué órdenes son rebotadas? Órdenes nuevas, modificaciones en órdenes ejecutadas (movimientos de _stop-loss_ o compras _limit_) y cambios en el _leverage_.

¿Qué órdenes ingresan instantáneamente sin tener en cuenta la cola de procesamiento? Cierres totales de posiciones de tipo _limit_, cierres de tipo _market_ (parciales o totales) y cancelaciones de órdenes.

¿Qué tenés que hacer para que tus órdenes se ejecuten siempre?

&#x20;

1. Definir los _stop-loss_ con anterioridad, tal y como mencioné algunas páginas atrás.
2. A) Cerrar las **posiciones completas** al ejecutarlas a precio limit.

B) Cerrar posiciones a partir de órdenes **market**.

&#x20;

Muchos traders esperan que Bitmex mejore en este sentido, pero a mi entender, este tipo de situaciones existen justamente para que usuarios novatos pierdan su dinero. Si seguís los consejos que di a lo largo de este capítulo, no deberías tener problemas al momento de operar.

Una vez más te recomiendo utilizar la _testnet_ de la plataforma el tiempo que creas necesario, y además ingresar a la real con un monto simbólico. Una vez que te sientas realmente cómodo operando en Bitmex, podés agregar más capital y disfrutar beneficios que no obtendrías en otras plataformas.
