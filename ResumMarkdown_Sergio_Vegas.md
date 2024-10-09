# Programació, entorns i processos

## Introducció a la programació

### Orígens de  programació

La programació s'ha desenvolupat al llarg dels anys gracies a la contribució de diferents persones com:
- Joseph Marie Jacquard
- Charles Babbage
- Ada Lovelace
- Alan Turing
- Grace Hopper
### LLenguatges de programació

Un llenguatge de programació és un llenguatge que permet establir una comunicació entre l’home i la màquina.
Es poden classificar segons: nivell d'abstracció del llenguatge i el tipus de traducció del programa al llenguatge de màquina.
#### Nivells d'abstracció dels llenguatges

Un **llenguatge de programació d'alt nivell** es caracteritza per expressar els algorismes d'una manera adequada a la capacitat cognitiva humana, en lloc de la capacitat amb què els executen les màquines. Exemples: C#, JAV, Python...

En un **llenguatge de programació de baix nivell**, en canvi, les seves instruccions exerceixen un control directe sobre el maquinari i estan condicionats per l'estructura física de les computadores que el suporten. Això no implica que siguin menys potents, sinó a la reduïda abstracció entre el llenguatge i el maquinari. Exemples: Llenguatge binari i assemblador.
#### Tipus de traducció dels programes

Els **llenguatges compilats** tradueixen (compilen) tot el codi font i contenen aquesta traducció en un arxiu executable comprensible per a la màquina en la plataforma en què s'ha compilat.L'arxiu només podrà ser executat en el mateix sistema operatiu en el que s’ha compilat.Exemples: C#,C,Pascal...

Els **llenguatges interpretats** tradueixen (interpreten) el codi font pas a pas, és a dir, instrucció per instrucció. La traducció del programa es repeteix cada vegada que s'executa el programa. Exemple: Python, JavaScript...

**Com codifica la informació l'ordinador?**Quan treballem amb números, acostumem a treballar en codificació decimal (en base 10). L'ordinador, en el seu nivell més baix, treballa en format binari (en base 2). No obstant, també farem servir altres tipus de codificacions: octal (en base 8) i hexadecimal (en base 16).
### Classificació dels llengautges i paradigmes de programació

#### Generacions dels llenguatges de programació

- **Llenguatge de primera generació**: Codi binari, de baix nivell.
- **Llenguatges de segona generació**: Assemblador, notacions llegibles.
- **Llenguatges de tercera generació**: D'alt nivell, fa falta compilador i s'assembla al llenguatge humà.
- **Llenguatges de quarta generació**: No procedimental, niveel molt alt d'asbtracció.
- **Llenguatges de cinquena generació**: IA.
#### Paradigmes de programació

Un paradigma de programació consisteix en els mètodes per dur a terme càlculs i en la forma en la qual han d'estructurar-se i organitzar-se les tasques que ha de realitzar un programa. Hi han dels següents tipus:

- **Programació imperativa o per procediments**
- **Programació orientada a objectes**
- **Programació dirigida per esdeveniments**
- **Programació declarativa**
- **Programació multiparadigma**
# Disseny d'algorismes

1. Anàlisis
2. Disseny
3. Programació
4. Compilació
5. Execució i proves
## Anàlisis

### Les dades
Una dada és una representació simbòlica (numèrica, alfabètica, …) d'una característica d’una entitat (un objecte de la vida real). No té valor semàntic (sentit) per si mateixa, però convenientment tractada (processada) es pot emprar en la realització de càlculs o presa de decisions. 

- **Simples**

    - numèriques

        - enter: representa un valor numèric, positiu o negatiu, sense cap decimal

        - real: representa un valor numèric, positiu o negatiu, amb decimals

    - no numèriques

        - booleà: representa un valor de tipus lògic per tal d’establir la certesa o falsedat d’un estat o afirmació

        - caràcter, cadena de caràcters: representa una unitat fonamental de text usada en qualsevol alfabet, un nombre o un signe de puntuació o exclamació
- **Estructurades**

    - internes

        - estàtiques (registres, vectors, taules)

        - dinàmiques (llistes, cues, piles, arbres)

    - externes

        - fitxers

        - bases de dades

### Les expressions

Una **variable** és una dada emmagatzemada en memòria que pot veure modificat el seu valor en qualsevol moment durant l’execució del programa.

Una **constant** és un tipus especial de variable que té la particularitat que dins del l'algorisme el seu valor només pot ser llegit, però mai modificat. 
![taula d'ordre de preferencia](http://insjoaquimmir.cat/wiki/images/thumb/b/b2/C_opassoc.png/300px-C_opassoc.png)

## Disseny
### Pseudocodi

El pseudocodi és una descripció a molt alt nivell de l'estructura d'un programa. L'algorisme s'encapsula dins de dues sentències, que marquen l'inici i el final de l'algorisme i delimiten les instruccions que el formen.
Les estructures condicionals controlen la seqüència d’execució d’altres instruccions, segons una determinada condició. Poden ser simples, dobles o múltiples:

- **Condició simple**



    if <condicio_certa> then

    instruccio_condicio_certa;

    endif


- **Condició doble**



    if <condicio_certa> then

    instruccio_condicio_certa;

    else	

    instruccio_condicio_falsa;

    endif

Les iteracions o bucles repeteixen un cert nombre de vegades les expressions que hi ha contingudes dins d’un algorisme. Segons la condició de repetició, hi ha tres tipus diferents d'estructures de repetició:

- **While (mentre)**

    while <condicio> do

        instruccio_1;

        instruccio_2;
	
    endwhile

- **Do...While (fer...mentre)**

    do	

        instruccio_1;	

        instruccio_2;

    while <condicio>;	

- **For (repetir)**


     for <vinicial> to <vfinal>

        instruccio_1;

        instruccio_2;

    endfor

### Diagrames de flux
El diagrama de flux (flowchart) és una representació gràfica simple de l'estructura d'un programa. Els diferents tipus d'operacions es representen a partir d'un determinat conjunt de símbols.
![Nomenclatura](![https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgWvPHwZfPeYkHSFaCXD_4E27atbIQfOhV9rNEmvj9UyLJpgMI7RR6N6gSlY62rRzfwhtjzKc7OYk2P-dXzLC5DLtEfK6gjJAzoTae0eRhzQD0Pg54WXF_ZS7eltd3IVwG74Amzrb25cSok/s640/Captura+de+pantalla+%252816%2529.png)
### Jocs de proves
A l’hora de dissenyar un algorisme, cal realitzar les proves necessàries per a avaluar la seva validesa. Els jocs de proves documenten els casos provats i els resultats obtinguts, per tal de corregir i millorar els programes.