# Eloquent Javascript 
## Chapter 1

### Eigenschaften von Javascript
* dynamisch und schwach typisiert
* Datentypen dynamisch zur Laufzeit ermittelt
* Typ kann sich zur Laufzeit ändern
* automatische Konvertierung von Typen
* funktionale Programmierung
* prototypische Objektorientierung

# 4 primitive Datentypen
1. Numbers

    * numerische Werte -> 64 bits -> 2 hoch 64 Nummern moeglich (18 Quintillion, 18 mit 18 Nullen)
    * 1 Bit bestimmt das Vorzeichen
    * ganze sowie Fliesskommazahlen  

    #### Schreibweisen
    * _dezimal_
    * _hexadezimal_ -> 0xffaa = 65450
    * _oktal_ -> 054 = 44
    * _exponential_ -> 1.5e3 = 1.5 * 1000
    * <span style="color:red">binaer geht nicht!</span>

    #### Spezielle Zahlen
    * Infinity/-Infinity
    * NaN

2. Strings

    * repraesentieren Text, kodiert in UTF-8 oder UTF-16
    * erlaubte Zeichen: " ", ' ', \` \`
    * <span style="color:red">Chars gibt es nicht</span>
    * backslash als Praefix fuer spezielle Zeichen
        Anweisung | Bedeutung
        ------- | -------
        | \n | New Line
        | \t | Tabulator
        | \\" | "
        | \\\ | \ | 
    
    #### Concatenieren
    * concateniert wird ueber den + Operator
    ```javascript
        "con" + "cat" -> concat
        "con" - "cat" -> NaN
    ```

    #### Backticks
    ```javascript
       `half of 100 is ${100/2}` -> half of 100 is 50 
    ```

    #### Unary Operator
    ```javascript
       console.log(typeof 4.5) -> Number
       //Minus kann unary und binary Operator sein (Rechnen und Negieren) 
    ```
    ```javascript
       console.log(typeof 42); // expected output: "number"
       console.log(typeof 'blubber'); //expected output: "string"
       console.log(typeof true); // expected output: "boolean"
       console.log(typeof declaredButUndefinedVariable); // expected output: "undefined"; 
    ```

    [typeof Beispiele](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators/typeof)

3. Boolean

    * Grossbuchstaben sind kleiner als Kleinbuchstaben (wegen ASCII Code)
    * Buchstaben werden von links nach Rechts Buchstabe fuer Buchstabe verglichen
    ```javascript
       NaN == NaN // -> false 
    ```
    
    Truly | Falsy
    ------- | -------
    | rest | undefined
    |  | leere Strings/Objekte
    |  | 0
    |  | NaN
    |  | null  

    ```javascript
       null == false // -> false 
       null == true // -> false
       undefined == false // -> false
       undefined == true // -> false
       NaN == true // -> false
       NaN == false // -> false 
    ```
    
    [Comparison Beispiele](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators)

    ![Javascript Humor](https://brunocapuano.files.wordpress.com/2018/07/thanks-for-inventing-javascript.jpg?w=500)

    ```javascript
       !true -> false
       !false -> true 
       console.log(null || "user") // -> user (da user truly und 0+1=1)
       console.log("Agnes" || "user") // -> Agnes, da bei 2 truly das linke ausgewertet wird
    ```

    #### automatische Typkonvertierung
    * bei Vergleichen z.B. koennten automatische Typkonvertierungen stattfinden
    * wird vermieden durch `=== oder !===`

4. Leer
    
    * null oder undefined
