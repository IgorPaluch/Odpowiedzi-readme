1.  
    P: Czym Jest hoisting i czy const podlega hoistingowi?

    Odp: Hositing to możliwość korzystania z zmiennych/deklaracji przed ich zdefiniowaniem w kodzie Hoisting - czyli przenoszenie na samą górę. Const nie podlega hoistingowi, możemy to zauważyć na przykładzie funkcji anonimowej przypisanej do consta np. const anonymousFunction = function() {}, nie możemy z niego korzystać zanim zostanie wywołany/zadeklarowany, natomiast sytuacja ma się już inaczej gdy posłużymy się function anonymousFunction(){}, z takiej funkcji możemy skorzystać zanim zostanie ona zadeklarowana w kodzie.
2. 
    P: Napisz w kilku zdaniach do czego służą middleware w Node.js

    Odp: funkcja, która jest uruchamiana za każdym razem, gdy przychodzi żądanie, np. Gdy chcielibysmy usunac uzytkownika, to jest potrzebne potwierdzenie jego autentykacji i dopiero za sprawą tego, możemy podjąć dane działanie.
3.  
    P: Napisz program w js, który będzie poprawnie parsował dane.
        Odp: Nie wiem czy taki rezultat autor zadania oczekiwał, natomiast opis tego zadania jest na tyle niezrozumiały, że przyjąłem, że dostaliśmy JSON, którego daliśmy do template stringa, a następnie funkcją za pomocą JSON.parse wyprowadzamy go do dwóch obiektów w tablicy. Rezultat można podejrzeć tutaj: https://codepen.io/IgorPaluch/pen/MWqvmxo?editors=1111

        const data = [   { "element": "1", "parametr": ["pierwszy", 1, "drugi", 2, "trzeci", 3]   },   { "element": "2", "parametr": [{ "1": 11 }, { "2": 11.34 }, { "3":   87.93 }] } ]

    const result = data.find(item => item.parametr);

    const secondResult = data.find(item => item.element === "2");

    const objSecondResult = Object.values(secondResult);

    let json = JSON.stringify(objSecondResult);

    console.log("Element: "+ parseInt(result.element) + "," + " Values: " + result.parametr);
    console.log("Element: "+ parseInt(secondResult.element) + "," + " Values: " + json )
4.  
    P: Co zostanie wyswietlone w konsoli?

    Odp: Odpowiedź (A) czyli undefined. Proces wygląda następująco czyli deklaracja, następnie wypisanie zminnej w console.log() a w ostatniej kolejności przypisanie wartości do zmiennej, dlatego też zmienną czyta jako zadeklarowaną, ale bez przypisanej wartości do niej.
5.  
    P: Do czego służy poniższa funkcja? 

    Odp: Nad tym pytaniem spędziłem chyba najwięcej czasu, zakładam, że jest to jakiś rodzaj ekstrapolacji matematycznej, ale naprawdę dziwna funkcja i do konca nie rozumiem jej działania.

6. Brak szóstego, ponieważ nigdy nie używałem tych bibliotek.
