# Margin trading

## MARGIN TRADING EN BITMEX

Por _margin trading_ se entiende a la práctica de utilizar fondos a préstamo al momento de comercializar activos financieros. A partir de esta modalidad se puede especular a que el valor de un activo aumente o disminuya su precio en el mercado, y a raíz de eso, maximizar beneficios o pérdidas a partir del capital adquirido en préstamo.

Tanto este capítulo como el próximo están dedicados al uso de la plataforma Bitmex porque es la que elegí y utilizo diariamente. Si pensás operar en otra, podés aplicar los conceptos, pero siempre teniendo en cuenta que cada exchange tiene sus particularidades y _mañas_. Dejando una consulta en el foro que forma parte del curso, podés charlar con el resto de lectores/as sobre otras plataformas (Binance, Bybit, Deribit, FTX, etc).

&#x20;

Bitmex (Bitcoin Mercantile Exchange) abrió sus puertas en el año 2014. Permite operar contratos a partir de las monedas BTC, ADA, BCH, EOS, ETH, LTC y XRP, y tiene ciertas particularidades respecto del resto de los _exchanges_:

&#x20;

\- **Protocolos de seguridad sólidos:** el almacenamiento de los fondos de la plataforma se realiza en fondos fríos (fuera de internet). Los retiros se realizan manualmente a las 13:00 UTC. El sitio cuenta con autentificación en dos factores -la cual recomiendo ampliamente utilizar- y cifrados extra, opcionales.

\- **Posibilidad de operar a** short**:** Bitmex es una de las primeras plataformas que soporta operaciones de ventas en criptomonedas a _short_. Esto permite obtener beneficios cuando se espera un descenso en el precio. Tal vez hayas leído algo sobre George Soros, quien en 1992 tumbó la libra esterlina y en 24 horas ganó mil millones de dólares operando _a la baja (_[4](https://es.wikipedia.org/wiki/Mi%C3%A9rcoles\_negro)).

\- Margin trade **(apalancamiento):** utilizando estrategias sólidas, puede otorgar beneficios muy rentables.

\- **Bajas comisiones:** la comisión de tipo _market_ es apenas más elevada que el promedio de Forex, por ejemplo, pero las órdenes _limit_ reciben comisión en vez de pagarla. Si trabajaste en Merval o en otros exchanges, las comisiones de Bitmex te va a parecer irrisorias. La plataforma no cobra por retiros ni depósitos.

**- Volumen:** está entre los exchanges de futuros de criptomonedas más líquidos, lo cual es estrictamente necesario, sobre todo al hacer _scalping_.

**- No KYC:** esto, a mi criterio, mantiene una diferencia sustancial frente a su competencia.

&#x20;

Bitmex no es técnicamente un _bróker_ sino un exchange descentralizado (_peer-to-peer_) para usuarios avanzados. El volumen diario que se mueve en la plataforma es de varios miles de millones de dólares; es el escenario ideal para que novatos pierdan su dinero y _traders_ experimentados obtengan beneficios.

No comisiona por depósitos o retiros (solo se cobra el _fee_ propio de la utilización del protocolo Blockchain) y esto lo convierte en el sitio ideal frente a quienes pretendemos lograr _profits_ y retirar ganancias de manera diaria o semanal.

Los depósitos generalmente se acreditan a los 15 o 20 minutos de iniciada la transacción y los retiros diariamente a las 10 AM (GTM -3, Argentina).

&#x20;

La web de Bitmex tiene a disposición un [manual muy bien desarrollado](https://www.bitmex.com/app/tradingOverview) donde se explica de manera detallada el funcionamiento del _exchange_ en su totalidad. Te recomiendo leerlo -desconozco por qué es tan común que la gente no lea manuales- porque aporta muchísima información.

&#x20;

**ES NECESARIO** que lo hagas.

&#x20;

En la imagen que adjunto a continuación muestro de qué manera organizo los paneles de la plataforma para tener a mano las herramientas que utilizo al momento de operar. Por supuesto que esto queda a tu criterio y solo tiene fines ilustrativos.

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption><p>Interfaz de Bitmex matenauta (adaptable a cada trader)</p></figcaption></figure>

## ¿BTC/XBT, CONTRATOS, FUTUROS?

Bitmex admite depósitos y retiros exclusivamente en BTC. El _exchange_ establece en su plataforma un sistema globalizado de _margin trading_ por lo cual las operaciones se realizan sobre contratos y no sobre criptomonedas. Los contratos pueden ser perpetuos (atados al dólar -BTC y ETH-) o futuros (_criptos_ restantes).

A modo personal te recomiendo operar futuros porque representan una volatilidad menor y además escapan al sistema de [funding fees](https://www.bitmex.com/app/perpetualContractsGuide) que la plataforma establece en contratos perpetuos.

&#x20;

La denominación BTC incumple con la norma ISO 4217 que establece la regla de tres dígitos para las divisas del mundo, por entrar en conflicto con la divisa BTN (unidad monetaria de Bután). Bitmex prefiere utilizar la denominación XBT frente al Bitcoin para prestar acuerdo con la norma ISO mencionada.

&#x20;

Cada contrato que se intercambia en el _exchange_, obtiene el valor de un dólar sobre esa moneda. A modo de ejemplo, si el valor del BTC es de U$S 10.000, cada contrato representaría un dólar y el conjunto de 10.000 contratos equivaldrían a 1 BTC.

Al operar con apalancamiento se disminuye la cantidad de contratos necesarios para abrir una posición y, de esa manera, se permite ampliarla a un monto mayor al depositado efectivamente en la cuenta.

La plataforma es una de las pocas que permite trabajar con _leverages_ arriba de 10X, las ganancias son ilimitadas pero las pérdidas nunca pueden superar la posición inicial. En esa situación el sitio cierra automáticamente la posición a pérdida, produciendo así una “liquidación” de la misma.

¿Cómo hace el sitio para ofrecer ganancias ilimitadas? A través de [Insurance Fund](https://www.bitmex.com/app/insuranceFund) que es sostenido justamente por posiciones liquidadas (_traders_ que operan a 50X o 100X esperando retornos fantásticos).

Bitmex obtiene cerca de 500 BTC semanales por liquidaciones en los usuarios que utilizan la plataforma. Luego te voy a comentar cómo podés mantenerte fuera de esa situación.

## LEVERAGE (APALANCAMIENTO)

No me voy a detener en explicar cómo funciona el _margin trading_ o el apalancamiento a nivel general -porque no es el objetivo del libro- pero sí voy a recomendarte que, incluso si ya trabajaste en otros mercados apalancando, comiences en esta plataforma con _leverages_ bajos (2 o 5X **máximo**).

**Siempre hay tiempo de obtener mejores** profits**.** Lo importante en principio es que no pierdas dinero de manera innecesaria, y ese debería ser tu principal objetivo durante tus primeros seis meses en el mercado.

La volatilidad de las criptomonedas es muy alta y utilizar _leverages_ por encima de 10X puede liquidar tu posición o generarte pérdidas realmente extraordinarias a partir de ejecuciones continuadas de _stop-loss_. Nos pasó a muchos, podés evitarlo.

&#x20;

La plataforma tiene mala reputación por este tipo de maniobras desde personas sin experiencia. Salvo que quieras apostar -lo cual va totalmente contra la mentalidad que debés desarrollar como _trader_-, te aconsejo NUNCA utilizar 50X o 100X. Los riesgos de liquidación de la posición en esos _leverages_ son realmente enormes y es desde donde prácticamente se sostiene la plataforma.

El retorno que podés calcular a 50X o 100X es extraordinario, pero con apenas un poco de paciencia y entradas claras, lo podés lograr con _leverages_ más bajos y sin asumir semejantes riesgos. En el siguiente gráfico podés observar variaciones de precio que liquidaron miles de posiciones:

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption><p>Liquidaciones en ETHUSD a 1H en Bitmex.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption><p>Múltiples liquidaciones en ETHUSD a 4H (Bitmex).</p></figcaption></figure>

En [BitmexRekt](https://twitter.com/bitmexrekt) (cuenta de Twitter) se publican en tiempo real las liquidaciones que se dan en la plataforma, tomando los datos desde la API del _exchange_, mientras que en [CryptoMeter](https://www.cryptometer.io/bitmex-rekt) se expresa la misma información de manera gráfica e intuitiva.

No es necesario que te expongas al mercado de esa manera. Más adelante te voy a dejar la información relevante para que evites ser parte de _los liquidados_.

## COMISIONES EN BITMEX

Las comisiones en la plataforma se cobran o pagan al momento de operar y se diferencian según el contrato y el tipo de órdenes que utilices. En [este link](https://www.bitmex.com/app/fees) las podés ver detalladamente.

Teniendo en cuenta la estrategia que desarrollo en el libro, voy a diferenciar las órdenes _taker_ de las órdenes _maker_ respecto de **contratos futuros**. Evito operar en contratos permanentes de BTC o ETH porque son demasiado volátiles y manejan [un fee extra](https://www.bitmex.com/app/perpetualContractsGuide) que no se paga en futuros.

Por órdenes _taker_ (órdenes market), se paga un **0,050% de comisión** en futuros de BTC y **0,25%** en futuros de _altcoins_.

Por órdenes _maker_ (órdenes limit), se **RECIBE** un **0,025% de comisión**. Sí, Bitmex paga comisión de órdenes _limit_.

## DESCUENTO DEL 10% EN COMISIONES

Si te registrás en Bitmex utilizando [este cupón](https://www.bitmex.com/register/4Nitpa) (_click_ para abrir la web de registro) obtenés un 10% de descuento en tus comisiones durante los primeros 6 meses.

Pasado ese período podés volver a registrarte utilizando otra casilla de e-mail y continuar con el beneficio. Bitmex admite múltiples cuentas de usuario, por lo que, si ya estás registrado al leer este libro, podés hacerlo nuevamente con otro _e-mail_ y comenzar a operar con descuento. Así es la magia del NO KYC (“Know Your Customer”, en inglés).

El **10% de descuento en las comisiones** parece no ser relevante, pero hay que tener en cuenta que ese monto se suma tanto en la entrada como en la salida (se cobra dos veces si se ejecutan dos órdenes _market_). Además, al trabajar realizando operaciones diarias apalancando, la diferencia realmente se hace notar porque el _leverage_ es tenido en cuenta al momento de la comisión.

Mi estrategia apunta a obtener retornos en períodos de tiempo reducidos, es fundamental pagar la menor comisión posible en cada transacción. Con el 10% de descuento, las órdenes _taker_ (o **market**) pagan solo **0.045%** de comisión en futuros de BTC y **0.225%** en _altcoins_.

## LA IMPORTANCIA DE LA TESTNET

Una de las características más interesantes de Bitmex frente a otras plataformas es que incorpora la posibilidad de abrir una cuenta de prueba, donde se puede operar a partir de depósitos en BTC ficticios.

Tal vez supongas que no es necesario, que ya conocés otras plataformas similares y Bitmex es una más del montón. Error.

&#x20;

Adquiriste este libro con el acceso a un foro privado de discusión donde vas a poder intercambiar ideas y consultas, tanto conmigo como con el resto de los lectores.

Salvo que ya hayas operado en Bitmex y realmente domines la plataforma, **ES NECESARIO** que abras una cuenta demo y la utilices. No voy a responder consultas que se puedan resolver con el aprendizaje que otorga la cuenta demo de la plataforma.

Es gratis y sencillo, sin riesgos. Podés probar los distintos tipos de órdenes: compras _limit_, compras _market_, _stop-loss limit/market. Trailing stops_, agregar o quitar _leverage_, mover órdenes desde el gráfico, etc.

&#x20;

Te aconsejo operar con pocos contratos ficticios (no con 1 BTC sino una fracción de satoshis) porque de lo contrario tu posición puede completarse en demasiado tiempo. La _testnet_ administra su propio volumen y no es tan elevado como el que maneja la plataforma original. El registro de usuario se realiza de manera independiente a Bitmex. Podés utilizar el mismo _e-mail_ en ambas versiones del _exchange_.

&#x20;

[Click para acceder a la testnet de Bitmex](https://testnet.bitmex.com/). Si aún no lo hiciste, **ES NECESARIO** que pruebes y aprendas a utilizar la plataforma.
