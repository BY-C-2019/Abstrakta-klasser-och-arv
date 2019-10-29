# Abstrakta-klasser-och-arv

I den här uppgiften ska du skriva ett enkelt program som kan hantera Rektanglar och Ellipser. De båda geometriska figurerna har vissa gemensamma attribut och metoder och dessa kan därför implementeras som en abstrakt basklass som vi kallar för Shape. De båda geometriska figurerna ska ärva från basklassen. 

## Klassen Shape
Shape ska vara abstrakt och det kommer därför inte gå att skapa några objekt av denna typ. Endast subklasserna Ellipse och Rectangle kommer gå att skapa objekt ifrån. Dessa båda klasser måste också implementera Area och Perimeter som är abstrakta properties. 
I klassen Shape ska det finnas två fält, length och width som är av typen double. Det ska finnas en publik metod ToString. Strängen som returneras ska vara på formatet: Legnth, Width, Perimeter & Area.

## Klassen Ellipse
Låt klassens konstruktor anropa basklassens konstruktor för att sätta längd och bredd. Implementera även Area och Perimeter.

## Klassen Rectangle
Implementeras på samma sätt som klassen Ellipse

## Program klass - EXTRA!
Vill du fortsätta med övningen kan du nu skriva en program klass. Förutom main metoden ska det finnas en del andra metoder för att hantera utskrifter och skapande av objekt i programmet. 

### Metoden CreateShape
Den här metoden ska användas för att skapa nya objekt av önskad typ. Typen anges genom att skicka in ett enum värde till metoden. 

### Metoden Main
Startpunkt för programmet som ska visa en meny med valmöjligheten att skapa någon av de typer som programmet stödjer samt att avsluta programmet. När ett val har gjorts ska ViewShapeInfo anropas för det skapade objektet.

### Metoden ViewShapeInfo
Gör en utskrift av objektets information genom ett anrop till dess toSrting() metod.

#### Kravlista:
1. Implementera klasserna Shape, Ellipse och Rectangle
2. Egenskaperna som kan sättas (har en set metod), width och length ska ha validering för felaktig indata
3. Lägg till nödvändiga metoder för menyutskrift, inläsning och utskrift på programklassen
4. Vid fel ska lättförståeliga felmeddelande skrivas ut

## Interface
Utöka prgroammet genom att skapa en version av Rectangle som går att ändra storlek på. Detta görs genom att skapa ett interface av type Resizable med metoden resize(int) som ska ändra storleken i procent. 
Skapa sedan en klass ResizeableRectangle som implementerar interfacet Resizable.
