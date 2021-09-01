<span class="bigTitle">JavaScript para gatos</span>
## Unha introdución para novos programadores <span class="right">![cat](images/substack-cats.png)</span>
### *Tan sinxelo que até teu compañeiro humano podería facelo!*

JavaScript é unha linguaxe de programación ou, noutras palabras, un medio polo cal se lle indica a unha computadora que faga cousas. Do mesmo xeito que un controla aos humanos con miadas e roncados, un controla ás computadoras con declaracións escritas nunha linguaxe de programación. Todos os navegadores web entenden JavaScript, así que podemos aproveitalo para facer que as páxinas web fagan cousas.

JavaScript comezou como un xeito de facer as páxinas web máis interactivas. Hoxe en día JavaScript funciona en máis lugares que nos navegadores web: funciona en servidores web, teléfonos e incluso robots. Imos revisar algúns conceptos básicos de JavaScript para que poidas aproveitalo en pouco tempo*.

\* *Tempo real: Probablemente unha ou dúas horas. Ademais, xa que es gato, tes menos probabilidades de sair correndo para deitarte ao sol*.

JavaScript for Cats is [CC0 Licensed](https://creativecommons.org/publicdomain/zero/1.0/)

## Táboa de contidos

- [A consola](#basics)
- [Strings](#strings)
- [Valores e variables](#values)
- [Empregando funcións](#functions)
- [Funcións JS incorporadas](#standard-library)
- [Descarga novas funcións JS](#third-party-javascript)
- [Escribindo novas funcións](#writing-functions)
- [Loops](#loops)
- [Arrays](#arrays)
- [Obxectos](#objects)
- [Callbacks](#callbacks)
- [Lecturas recomendables](#recommended-reading)

## Non sexas un gato medrento

<span class="right">![cat](images/yarnify.png)</span>

Sempre caerás de pé, inda cando programes. A diferenza de tirar un vaso de auga encima do portátil, *nada* destas prácticas danará o teu ordenador de ningún xeito, aínda que escribas mal un comando ou fagas clic no botón incorrecto. Do mesmo xeito que os gatos, os programadores cometen erros todo o tempo: escriben mal as cousas, esquecen as comiñas ou as parénteses e esquecen o funcionamento das funcións básicas. Os programadores se preocupan máis de *finalmente* facelo funcionar, que de tentar facelo funcionar á primeira. Así que a mellor maneira de aprender, coma non, é cometendo erros.

Así que non sexas gato medrento. O peor que pode suceder é que teu navegador se colgue. Inda así, non te preocupes, isto ocorrerá ben poucas veces.

## <a id="basics" href="#basics">#</a> O básico

*Podes limitarte a ler o artigo, pero se pensas practicar os exemplos, e só por motivos de sinxeleza, emprega Google Chrome.*

Agora, neste momento, JavaScript estase a executar nesta páxina. Xoguemos un pouco con el. 

Primeiro, fai clic co botón dereito en calquera lugar da pantalla e fai clic en **Inspeccionar elemento** e logo fai clic na pestana **Consola** . Deberías ver unha cousa que ten este aspecto:

![console](images/console.gif)

Trátase da consola, tamén coñecida como "liña de comandos" ou "terminal". Basicamente é un xeito de escribir nun ordenador unha cousa á vez de obter de inmediato a resposta do mesmo. Son moi útiles como ferramenta de aprendizaxe (aínda uso a consola case todos os días que estou a codificar) e tamén de desenvolvemento.

A consola fai cousas ben cucas. Comeza a escribir algo e a consola axudarache dándoche unha lista de todas as cousas posibles que poderías seguir escribindo. Outra cousa que podemos facer é escribir na consola `1 + 1` e despois premer na tecla `Enter` e ver o que pasa.

O uso da consola é unha parte moi importante na aprendizaxe de JavaScript. Se non sabes se algo funciona ou cal é o comando para algo, vai á consola e descúbreo. Aí van uns exemplos:

### <a id="strings" href="#strings">#</a> Strings

Strings, cadeas ou cordas. 

*- Dende que son gato, quero substituír cada instancia en Internet da palabra `dog`  por `those blasted dogs`.*

Primeiro entro na consola e escribo algunhas frases que conteñan a palabra `dog` polo menos unha vez. En JavaScript, unha chea de letras, números, palabras ou calquera outra cousa coñécese como **string** - unha **cadea**, como nunha *cadea* de caracteres-. As cadeas teñen que comezar e rematar con comiñas. Simples `'`ou dobres `"`. Asegúrate de usar as mesmas ao principio e ao final de cada cadea.

![console](images/console-strings.gif)

Ves a mensaxe de erro? Non te preocupes, non incumprimos ningunha lei. SyntaxError ILLEGAL é o xeito que teñen os robots de dicir que o teu programa ten un problema. As dúas primeiras frases tiñan comiñas coincidentes ao comezo e ao final, pero cando mesturámolas comiñas simples e dobres salta o erro.

Está ben, para arranxar unha destas frases (substituíndo `dog` pola nova versión mellorada) primeiro temos que gardar a frase orixinal para logo poder chamala cando fagamos a maxia da substitución. Ves como cada string se repite en vermello cando o escribimos na consola? Isto ocorre porque non lle dixemos que gardase a frase en ningún sitio, polo que só a devolve e punto (ou, se desordenamos algo, devólveranos un erro).

### <a id="values" href="#values">#</a> Valores e variables

Os **valores** son os compoñentes máis sinxelos de JavaScript. `1` é un valor, `true` é un valor, `"hello"` é un valor, `function() {}` é un valor, e a lista continúa. Hai un puñado de diferentes **tipos** de valores en JavaScript, pero non precisamos repasalos todos de inmediato; aprenderémolos de xeito natural canto máis escribamos código.

Para almacenar valores empregamos as chamadas **variables** . A palabra "variable" significa "pode cambiar" e úsase porque as variables poden almacenar moitos tipos diferentes de valores e poden cambiar o seu valor moitas veces. Son case como caixas de correo. Poñemos algo nunha variable, como a nosa frase, e despois damoslle á variable un enderezo que podemos usar para buscar a frase máis tarde. Nas caixas de correo da vida real deben ter números de caixa postal, pero en JavaScript normalmente só se usan letras minúsculas ou números sen espazos.

![console](images/console-variables.gif)

`var` é abreviación de variable e os signos ``=`` do medio *almacenan a cousa á dereita na cousa á esquerda* . Como podes ver, agora que almacenamos a frase nunha variable, a consola xa non devolve a frase de inmediato, senón `undefined` que nos indica que *non había nada que devolver* .

Se agora escribimos un nome de variable na consola, imprimirá o valor almacenado nesa variable. Unha nota sobre as variables é que **por defecto desaparecen cando cambias a outra páxina**. Se tocas o botón Actualizar de Chrome (AGORA NON!), por exemplo, a variable `dogSentence` se borraría e sería coma se nunca existise. Pero, por agora; mentres permanecemos na consola con só tocar as frechas :arrow_up_small: ou :arrow_down_small: do teclado podemos percorrer todo o que introducimos recentemente.
### <a id="functions" href="#functions">#</a> Funcións

Agora que xa témola frase almacenada nunha variable, imos cambiar algunha palabra almacenada nela. Podemos facelo creando unha *función*. *As funcións* son un tipo de valor que, ben, serven para nós unha *función* específica (propósito ou acción). Supoño que chamalas simplemente "accións" pareceulles estraño, así foi que se as diferenciou coa palabra "function".

JavaScript ten unha función chamada `replace` que fai exactamente o que queremos. As funcións toman calquera número de valores entre parénteses (cero, un ou moitos) e non devolven nada ( `undefined` ) nin a cadea modificada. Unha función `replace` está dispoñible para usala en calquera cadea e inclúe dous valores: os caracteres para sacar e os caracteres para intercambiar. É confuso describir estas cousas polo que aquí tes un exemplo visual:

![console](images/console-replace.gif)

Ter en conta que o valor de `dogSentence` é o mesmo despois de que executemos `replace`? Isto débese a que a función `replace` (e a maioría das funcións JavaScript ao respecto) toma o valor que lle damos e devolve un **novo valor** , sen modificar o valor que pasamos. Dado que non gardamos o resultado (non hai ningún `=` ao lado esquerdo da función de substitución) a función so vai a imprimir o valor devolto na consola.

### <a id="standard-library" href="#standard-library">#</a> A "biblioteca estándar"

Pode que te preguntes que outras funcións están dispoñibles en JavaScript. A resposta: UNHA TONELADA. Hai moitas **bibliotecas estándar incorporadas** que podes aprender en MDN (un sitio administrado por Mozilla que ten moita información sobre tecnoloxías web). Por exemplo, [aquí está a páxina MDN sobre o obxecto Math de JavaScript](https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Global_Objects/Math).

### <a id="third-party-javascript" href="#third-party-javascript">#</a> JavaScript de terceiros

Tamén hai moito código JavaScript dispoñible que **non** está **integrado** . O JavaScript de terceiros normalmente denomínase "biblioteca" ou "complemento". Un dos meus favoritos chámase **Underscore.js**. Imos collelo e cargalo na nosa páxina. Primeiro vai ao sitio de Underscore, http://underscorejs.org/ , fai clic na ligazón de descarga (normalmente uso versións de desenvolvemento porque son máis fáciles de ler pero ambas nos darán a mesma funcionalidade básica) e despois copiar todo o código no portapapeis (podes usar Seleccionar todo no menú Editar para seleccionalo todo). A continuación, pégao na consola e preme 'Intro' . Agora o teu navegador ten unha nova variable: `_`. O subliñado ofrécenos unha chea de funcións útiles para xogar. Xa aprenderemos máis adiante como usalos.

![console](images/underscore.gif)

### <a id="writing-functions" href="#writing-functions">#</a> Facendo novas funcións

Non estamos limitados a usar funcións doutras persoas, tamén podemos escribir as nosas. É bastante fácil! Imos facer unha función chamada `makeMoreExciting` que engade unha morea de signos de exclamación ao final dunha cadea.
    
    ```js
      function makeMoreExciting(string) {
      return string + '!!!!'
    }
    ```

Que en voz alta lese algo así: *"hai unha función chamada  `makeMoreExciting` que leva unha cadea e devolve unha nova copia desa cadea ``+``  unha chea de signos de exclamación ao final"*. Vexamos como escribiríamos isto na consola manualmente se non estivésemos a usar unha función:

![console](images/custom-function-manually.gif)

A expresión `string + '!!!!'` devolve unha nova cadea e a nosa variable chamada `string` mantense como antes (xa que nunca a actualizamos a outra cousa `=` ).

Usemos a nosa función en vez de facelo manualmente. Primeiro, pegamola función na consola e despois **chamamos** á función **pasando** unha cadea:

![console](images/custom-function-call.gif)

Tamén podes chamar á mesma función pasando unha variable que apunte a unha cadea (no exemplo anterior acabamos de escribir a cadea alí como un valor en lugar de gardala primeiro nunha variable):

![console](images/custom-function-call-variable.gif)

A liña `makeMoreExciting(sentence)` equivale a dicir `sentence + '!!!!'`. E se quixésemos **modificar no lugar** (tamén coñecido como actualización) o valor da frase? Simplemente garde o valor de retorno da función na  variable `sentence`:

    ```js
    var sentence = "time for a nap"
    sentence = makeMoreExciting(sentence)
    ```

Agora `sentence` terá os signos de exclamación ao final. Ten en conta que só tes que usar `var` cando estás **inicializando** unha variable: a primeira vez que a usas. Despois diso non debes usar `var` a menos que queiras reinicializar (restablecer / borrar / baleirar) a variable.

Que pasaría se sacásemos a declaración `return` na nosa función?

![console](images/custom-function-no-return.gif)

Por que está `sentence` baleiro? Porque as funcións devolven `undefined` por defecto. Podes optar por devolver un valor `return` engadindo algo. As funcións deberían ter un valor e, se cambian o valor ou crean un novo valor que se supón que se usará despois: un valor `return` (soa divertido: un termo elegante para este estilo é a *programación funcional* ). Aquí hai outra función que non devolve nada senón que usa un método diferente para amosarnos a saída:

```js
function yellIt(string) {
  string = string.toUpperCase()
  string = makeMoreExciting(string)
  console.log(string)
}
```

Esta función `yellIt` usa a nosa función anterior `makeMoreExciting`, así como o método de cadea incorporado [toUpperCase](https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Global_Objects/String/toUpperCase) . Os métodos son só un nome para unha función cando pertence a algo - neste caso `toUpperCase` é unha función á que pertence a `String` así que podemos referirnos a ela como método *ou* función. `makeMoreExciting` por outra banda non pertence a ninguén así que sería técnicamente incorrecto referirse a ela como un método (confuso, si bastante, seino).

A última liña da función é tamén outra función incorporada que simplemente toma os valores que lle damos e os imprime na consola.

![console](images/custom-function-console-log.gif)

Entón, hai algún erro coa función anterior `yellIt`? Depende! Aquí están os dous tipos principais de funcións:

- funcións que modifican ou crean valores e os devolven
- funcións que toman valores e realizan algunha acción que non se pode devolver

`console.log` é un exemplo do segundo tipo de función: imprime cousas na túa consola, unha acción que podes ver cos teus ollos pero que non se pode representar como un valor JavaScript. A miña propia regra é tratar de manter os dous tipos de funcións separados entre si, así que aquí volvería escribir a función `yellIt`:

```js
function yellIt(string) {
  string = string.toUpperCase()
  return makeMoreExciting(string)
}

console.log(yellIt("i fear no human"))
```

Deste xeito `yellIt` tórnase máis **xenérico** , é dicir, só fai unha ou dúas pequenas cousas sinxelas e non sabe nada sobre a impresión propia nunha consola; esa parte sempre se pode programar máis tarde, fóra da definición da función.

### <a id="loops" href="#loops">#</a> Loops

Agora que temos algunhas habilidades básicas no peto. Podemos comezar a ser preguiceiros. Que?! Si, é certo: programar consiste en ser preguiceiro. Larry Wall, inventor da linguaxe de programación Perl, chamou a preguiza a [virtude máis importante](http://c2.com/cgi/wiki?LazinessImpatienceHubris) dun bo programador. Se non existisen computadores terías que facer todo tipo de tarefas tediosas a man, pero se aprendes a programar podes poñerte ao sol todo o día mentres un ordenador nalgún lugar executa os teus programas para ti. É un estilo de vida glorioso cheo de relaxación.

Os bucles son unha das formas máis importantes de aproveitar a enerxía dun ordenador. Lembras `Underscore.js` dalgún paso anterior? Asegúrate de telo cargado na páxina (lembra: só podes premer a frecha cara arriba no teclado algunhas veces e despois premer `Enter` para cargalo de novo se o precisas) e intenta copialo/pegalo na túa consola:
  
```js
function logANumber(someNumber) {
  console.log(someNumber)
}
_.times(10, logANumber)
```

Este código usa o método [times](http://underscorejs.org/#times) de Underscore que leva 1 número e 1 función e despois comeza desde 0 e durante 10 pasos conta 1, chamando á función co número a cada paso do camiño.

![console](images/times-loop.png)

Se escribísemos manualmente o que `times` está a facer no código anterior, quedaría así:

```js
logANumber(0)
logANumber(1)
logANumber(2)
logANumber(3)
logANumber(4)
logANumber(5)
logANumber(6)
logANumber(7)
logANumber(8)
logANumber(9)
```

Pero os gatos néganse a facer traballos manuais innecesarios coma este, polo que sempre debemos preguntarnos: *"Estou facendo isto do xeito máis preguiceiro posible?"* .

Entón, por que se chama isto looping? Pénsao así: se escribísemos unha lista de 10 números (de 0 a 9) usando un array JavaScript tería o seguinte aspecto:

```js
var zeroThroughTen = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

O que realmente fai `times` é visitar cada número e repetir unha tarefa: no exemplo anterior a tarefa consistía en chamar á función `logANumber` co número actual. Repetir tarefas deste xeito denomínase *looping sobre* a matriz.

### <a id="arrays" href="#arrays">#</a> Arrays

Ou matrices. Xa as levamos visto algunhas veces, pero imos dedicarlles un minuto. Imaxina que necesitas facer un seguimento de todos os teus amigos. Ben, un 'array' farache moito ben. Pensa nun 'a'rray' como nunha lista ordenada na que podes gardar *toneladas* de cousas.

Así facemos unha:

```js
var myCatFriends = ["bill", "tabby", "ceiling"]
```

Doce! Agora tes unha lista dos teus amigos gato.

Os elementos (isto é cada elemento único nunha matriz) que se almacenan dentro de matrices comezan en 0 e contan desde alí. Así que `myCatFriends[0]` devolve `bill`, e `myCatFriends[1]` devolve `tabby`... etc etc.

Para sacar amigos da túa matriz, só tes que acceder a un elemento así: 

```js
console.log(myCatFriends[0])
```

![console](images/array-access.png)

Se unha noite fas un novo amigo gato no coñecido Club Gato e queres engadilo á túa lista é moi sinxelo: `myCatFriends.push("super hip cat")`.

Para comprobar que o novo gato entrou na túa matriz, podes usar `.length`:

![console](images/array-push-length.png)

Ves como `push` devolve a lonxitude? A man! Ten en conta tamén que as matrices sempre **conservarán a orde**, o que significa que recordarán a orde na que engadiches ou definiches cousas. Non todo o JavaScript conserva a orde, así que recorda esta propiedade especial dos 'arrays'.
  
### <a id="objects" href="#objects">#</a> Obxectos

Os arrays son bos para listas, pero para outras tarefas poden ser difíciles de usar. Vexamos a nosa variedade de amigos gato. E se tamén quixeramos almacenar algo máis que nomes?

```js
var myCatFriends = ["bill", "tabby", "ceiling"]
var lastNames = ["the cat", "cat", "cat"]
var addresses = ["The Alley", "Grandmas House", "Attic"]
```

Ás veces é bo ter todos os enderezos ou nomes nunha variable. Pero ás veces tes un gato en mente, digamos Bill, e só queres buscar o enderezo dese gato. Con matrices leva moito traballo porque non se pode dicir "hey array, dame o enderezo de Bill" porque "Bill" está nunha matriz e o seu enderezo está nunha matriz totalmente diferente.

![console](images/array-lookup.png)

Isto pode ser fráxil porque se as nosas matrices cambian e engadimos un novo gato ao principio, tamén teríamos que actualizar a posición da variable `bill` para apuntar á nova localización da información de Bill nas matrices. Pero aquí tes un xeito máis sinxelo de manter información como esta empregando obxectos:

```js
var firstCat = { name: "bill", lastName: "the cat", address: "The Alley" }
var secondCat = { name: "tabby", lastName: "cat", address: "Grandmas House" }
var thirdCat = { name: "ceiling", lastName: "cat", address: "Attic" }
```
  
Por que o faríamos deste xeito? Porque agora temos unha variable para cada gato que podemos usar para que os velos gatos dun xeito máis cómodo e lexible.

![console](images/object-lookup.png)

Podes pensar nos Obxectos como chaves nun chaveiro. Cada unha é para unha porta específica e se tes etiquetas especificas nas chaves podes abrir as portas moi rápido. En detalle, as cousas do lado esquerdo do signo `:`  chámanse **keys** (ou tamén se coñecen como **propiedades** ) e as do lado dereito son *os seus* **valores**.

```js
// an object with a single key 'name' and single value 'bill'
{ name: 'bill' }
```

Entón, por que empregaríamos matrices se só podemos colocar os datos en obxectos? Porque **os obxectos non lembran a orde das propiedades(keys) que configuramos**. Podes introducir un obxecto coma este:

```js
{ date: "10/20/2012", diary: "slept a bit today", name: "Charles" }
```

Pero o ordenador podería devolvelo así:

```js
{ diary: "slept a bit today", name: "Charles", date: "10/20/2012" }
```

Ou así!

```js
{ name: "Charles", diary: "slept a bit today", date: "10/20/2012" }
```

Non podemos confiar nunca na orde das propiedades(keys) dos obxectos. Se queremos estar realmente á moda, podemos facer unha matriz chea de obxectos ou un obxecto cheo de matrices.

```js
var moodLog = [
  {
    date: "10/20/2012",
    mood: "catnipped"
  }, 
  {
    date: "10/21/2012",
    mood: "nonplussed"
  },
  {
    date: "10/22/2012",
    mood: "purring"
  }
]

// ordered from least to most favorite
var favorites = {
  treats: ["bird sighting", "belly rub", "catnip"],
  napSpots: ["couch", "planter box", "human face"]
}
```

Cando combinamos diferentes cousas coma estas, estamos a crear **estruturas de datos** , coma se foramos entendidos :heart_eyes_cat:.!

### <a id="callbacks" href="#callbacks">#</a> Callbacks - Devolucións de chamada

As devolucións de chamada non son realmente unha característica de JavaScript como `Object` ou `Array`, senón **un xeito de usar funcións**. Para comprender por que son útiles as devolucións de chamada, primeiro temos que aprender sobre a programación asíncrona (moitas veces acurtada a *async*). O código asíncrono por definición é o código escrito dun xeito que non é síncrono :smile_cat: . O código síncrono é fácil de entender e escribir. Aquí tes un exemplo para ilustralo:

```js
var photo = download('http://foo-chan.com/images/sp.jpg')
uploadPhotoTweet(photo, '@maxogden')
```

Este [pseudo-código](http://simple.wikipedia.org/wiki/Pseudocode) síncrono descarga unha adorable foto dun gato adorable e logo carga a foto en twitter e envía a foto ao Twitter de`@maxogden`. Semella sinxelo!

( *Nota do orixinal: @maxogden acepta tweets de fotos de gato ao azar* )

Este código é síncrono porque para que a foto se cargue no tweet, a descarga de fotos debe completarse. Isto significa que a liña 2 non pode executarse ata que a tarefa da liña 1 estea completamente rematada. Se realmente implementásemos este pseudo-código quereríamos asegurarnos de que a execución `download` se "bloquea" ata que remate a descarga, o que significara que evitarase que se execute *calquera* outro JavaScript ata que remate e, cando finalice a descarga, recuperaríase a execución de JavaScript e se executaría a liña 2.

O código síncrono está ben para as cousas que suceden rápido, pero é nefasto para as cousas que requiren gardar, cargar, descargar ou subir. Que pasa se o servidor desde o que descargas a foto é lento ou a conexión a internet que estás a usar é lenta ou o ordenador no que estás a executar o código ten demasiadas pestanas de youtube con vídeos de gatos abertas e funciona lentamente? Significa que pode levar uns minutos de espera antes de que a liña 2 chegue a correr. Mentres tanto, debido a que se bloquea a execución de todos os JavaScript da páxina mentres se está a facer a descarga, a páxina web conxelaríase totalmente e deixaría de responder ata que finalice a descarga.

Debería evitarse a toda costa a execución do bloqueo, especialmente cando facelo fai que o noso programa se conxele ou non responda. Supoñamos que a foto anterior tarda un segundo en descargarse. Para ilustrar canto tempo dura un segundo para un ordenador moderno, aquí tes un programa que proba para ver cantas tarefas pode procesar JavaScript nun segundo.

```js
function measureLoopSpeed() {
  var count = 0
  function addOne() { count = count + 1 }

  // Date.now() returns a big number representing the number of
  // milliseconds that have elapsed since Jan 01 1970
  var now = Date.now()

  // Loop until Date.now() is 1000 milliseconds (1 second) or more into
  // the future from when we started looping. On each loop, call addOne
  while (Date.now() - now < 1000) addOne()
  
  // Finally it has been >= 1000ms, so let's print out our total count
  console.log(count)
}

measureLoopSpeed()
```

Copiamos e pegamos o código anterior na consola JavaScript e despois dun segundo deberíase imprimir un número. Na miña computadora conseguín `8527360`, aproximadamente, **8,5 millóns**. Nun segundo JavaScript pode chamar á función `addOne` 8,5 millóns de veces. Entón, se temos un código síncrono para descargar unha foto e a descarga de fotos leva un segundo, significa que estamos a impedir que ocorran 8,5 millóns de operacións mentres a execución de JavaScript está bloqueada.

Algunhas linguaxes teñen unha función chamada `sleep` que bloquea a execución durante algúns segundos. Por exemplo, aquí hai algún código  [`bash`](http://en.wikipedia.org/wiki/Bash_(Unix_shell))  correndo en `Terminal.app` que se usa en Mac OS e que usa `sleep`. Cando executamos o comando `sleep 3 && echo 'done sleeping now'` se bloquea durante 3 segundos antes de imprimir `done sleeping now`.

![console](images/bash-sleep.png)

JavaScript non ten unha función `sleep`. Logo: "Por que estou aprendendo unha linguaxe de programación que non implica durmir?".  En vez de confiar en `sleep` e esperar a que ocorran cousas, o deseño de JavaScript fomenta o uso de funcións. Se tes que esperar a que finalice a tarefa A antes de facer a tarefa B, pon todo o código da tarefa B nunha función e só chamarás a esa función cando remate A.

Por exemplo, este é un estilo de código con bloqueo:

```js
a()
b()
```

E, este un estilo que non bloquea:

```js
a(b)
```

Na versión sen bloqueo `b` hai unha devolución de chamada a `a`. Na versión con bloqueo `a` e `b` os dous son chamados/invocados (ambos teñen despois `()` e executan as funcións inmediatamente). Na versión sen bloqueo só se invoca `a` , e `b` simplemente se pasa como argumento de `a`.

Na versión de bloqueo, non hai unha relación explícita entre `a` e `b`. Na versión sen bloqueo convértese en tarefa de `a`  que fará o que teña que facer e despois chamará a `b` cando remate. Usar funcións deste xeito chámase _**devolución de chamada**_ porque a súa función e devolver a chamada de execución. Neste caso chámase a  `b`,  máis tarde, cando `a` remate.

Aquí vai unha implementación de pseudocódigo do que podería ser `a`:

```js
function a(done) {
  download('https://pbs.twimg.com/media/B4DDWBrCEAA8u4O.jpg:large', function doneDownloading(error, png) {
    // handle error if there was one
    if (err) console.log('uh-oh!', error)
    
    // call done when you are all done
    done()
  })
}
```

Volva ao noso exemplo de non bloqueo, `a(b)` onde chamamos a  `a` e pasamos `b` como primeiro argumento. Na definición de función `a` anterior, o argumento `done`  que pasamos é a nosa función `b` . Este comportamento é algo difícil de meter na cachola ao principio. Cando chamas a unha función, os argumentos que pasas non terán os mesmos nomes de variables cando están na función. Neste caso o que chamamos `b` chámase `done` dentro da función. Pero `b` e `done` son só nomes de variables que apuntan á mesma función subxacente. Normalmente as funcións de devolución de chamada están etiquetadas como algo `done` ou `callback` para deixar claro que son funcións que se deben chamar cando se faga a función actual.

Así, `a` fai o seu traballo e chama a `b` cando remata,  e tanto `a` coma `b` se van a obter en ambas versións con bloqueo e sen bloqueo. A diferenza é que na versión sen bloqueo non temos que deter a execución de JavaScript. En xeral, o estilo sen bloqueo é onde escribes todas as funcións para que se poidan executar canto antes, sen se bloquear nunca.

Para levantar inda un piso máis a casa: se utilizas a versión con bloqueo e `a` tarda un segundo en completarse , significa que só podes facer esa cousa. Se utilizas a versión sen bloqueo (tamén chamada devolución de chamada), podes facer *literalmente millóns* de cousas nese mesmo segundo, o que significa que podes rematar o teu traballo millóns de veces máis rápido e durmir o resto do día.

Lembrar: a programación é unha cuestión de preguiza e hai que durmir, non sobre o ordenador.

Con sorte, agora podes ver que as devolucións de chamada son só funcións que chaman a outras funcións despois dalgunha tarefa asíncrona. Exemplos comúns de tarefas asíncronas son cousas como ler unha foto, descargar unha canción, cargar unha imaxe, falar cunha base de datos, esperar a que un usuario toque unha tecla ou faga clic sobre algo, etc. Todo o que leva tempo. JavaScript é realmente estupendo para xestionar tarefas asíncronas coma estas sempre que se tome o tempo para aprender a usar as devolucións de chamada e evitar que se bloquee o noso guión.

## De remate!

Este é só o comezo da túa relación con JavaScript. Non podes aprendelo dunha soa vez, pero debes atopar o que che funciona e tentar aprender os conceptos expostos aquí.

Recomendaríache volver mañá para repasar todo dende o principio. Pode levar algunhas veces antes de conseguir facernos con todo (a programación é difícil). Simplemente intenta evitar ler esta páxina en calquera cuarto que conteña obxectos brillantes. . . podente distraer indefectiblemente.

Tes outro tema que queres ver tratado? Abre un asunto [en Github](http://github.com/nunhes/javascript-for-cats), ou no orixinal tamén [en Github](http://github.com/maxogden/javascript-for-cats).

### <a id="recommended-reading" href="#recommended-reading">#</a> Lectura recomendada

JavaScript For Cats evita moitos detalles que non son importantes para encetar (os gatos non son coñecidos pola súa atención), pero se tes ganas de mergullarte máis fondo, comproba estas referenzas:
  
  - [NodeSchool.io](http://nodeschool.io/) é un software educativo de código aberto dirixido pola comunidade que ensina varias habilidades de desenvolvemento web nun formato interactivo e autoguiado. 
  - [Eloquent Javascript](http://eloquentjavascript.net/)  é un libro gratuíto que che ensina JavaScript. Está bastante ben! Especialmente o capítulo sobre [valores, variables e control de fluxo](http://eloquentjavascript.net/chapter2.html)
  - [Mozilla's JavaScript Guide](https://developer.mozilla.org/en-US/docs/JavaScript/Guide) tamén ten un capítulo introdutorio moi saboroso chamado [valores, variables e literais](https://developer.mozilla.org/en-US/docs/JavaScript/Guide/Values,_variables,_and_literals)
  - [`standard` JS Style Guide](https://github.com/feross/standard) é un *empaquetado* - linter- de "configuración cero" para o estilo JS
  - [Let's Write Code by @shama](https://github.com/shama/letswritecode) unha gran serie de tutoriais de codificación de YouTube feitos por alguén que sabe

<hr>

*a rough translation of [javascript-for-cats](http://github.com/maxogden/javascript-for-cats)*

*JSForCats.com is a labor of love and work in progress by [@maxogden](http://twitter.com/maxogden). If you would like to contribute and make this tutorial better there is a Github repo [right over here](http://github.com/maxogden/javascript-for-cats).*
