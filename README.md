# home-codeingStandardsRefactoring-EStr

## Ausarbeitung Refactoring

### Was ist Refactoring

Refactoring ist wenn der Code gereinigt wird. Dies kann in mehreren Varianten
passieren. Das Ziel damit ist den Code verständlicher zu machen, bzw. für die Zukunft verständlich halten. Dies kann gemacht werden, indem man
Kommentare einfügt, nicht genützter Code wird entfernt, Zahlen die aus dem nichts genommen werden (magical values)
ihren Sinn definiert wird, und weitere.

### Vorteil/Nachteil von Refactoring

Prinzipiell ist es ein Vorteil seinen Code zu refactoren, da es damit für die
Zukunft dann leichter ist den Code wieder zu benützen, oder an dem Projekt
weiterzuarbeiten. Denn es besteht die sehr hohe Wahrscheinlichkeit, dass du
dir dann nicht mehr zu 100% sicher bist, wo was gemacht wird, ohne dich vorher
richtig einzulesen.

Jedoch kann es sehr schnell passieren, dass der Code, obwohl du eigentlich
nichts getan hast, außer ihn zu reinigen, dann nicht mehr vollständig
funktioniert.
Desweiteren ist der Code dadurch auch leichter lesbar für andere Leute, was
ein Vorteril, sowie ein Nachteil sein kann.

### Welche Schritte werden beim Refactoring durchgegangen?

Beim Refactoren ist es nicht so wicthig, in welcher Reihenfolge du etwas machst,
als wie wichtig ist, dass du erstens, jeden schritt unabhängig voneinander machst,
also immer nur eine Sache auf einmal, und diesen danach testet, ob er noch 
funktioniert. Für den Fall, dass dieser dann nicht mehr funktionieren sollte,
ist es wichtig das du deinen Code während des Refactorens stets backupst, mit
zB GitHub.

### Prinzipien von guten Code

Es gibt mehrere Prinzipien von guten Code, die mit Merkhilfen versehen sind
und auch verständlich, trotzdem werde ich sie hier für Sie, noch einmal kurz erklären.

DRY - Don't Repeat Yourself
Du hast einen Code, bzw. eine Funktion mehrmals? Schaue das sie dann nur
einmal im Code steht und du diesen mehrmals benützt, wenn nötig

KISS - Keep It Simple, Stupid
Warum kompliziert wenn es auch einfach geht?

YAGNI - You Ain't Gonna Need It
Schreibe Code auch nur dann, wann du ihn benötigst, denn du weißt nie, was
passieren könnte

Principle of least Astonishment
Benenne deine Funktionen auch nachdem, was sie tun, lass es keine Überaschung sein

SoC - Seperation of Concerns
Dies ist hauptsächlich nur wichtig wenn mit, vorallem für, anderen Leuten gearbeitet wird.
Was im Grunde besagt, dass du immer bei Unsicherheiten vorher nachfragen sollst,
damit du am Ende nicht mehr Zeit in das Projekt steckst, wie für das Geld geplant war.

 ### Code smells?

Wenn ein Code stinkt, meint man das er schlecht ist. Was man unter einem schlechten
Code verstehen könnte, ist im Grunde ein unrefactored Code, außer vielleicht der
von einem ehrfahrenen Coder.
Was darunter fällt sind, zu lange Methoden (lass sie nicht länger wie ~25 Zeilen werden), 
magical Values/Strings, keine beschreibenden Kommentare und mehr.

### 10 Code smells, die mich betreffen könnten

1. keine Kommentare - beschreibende Kommentare machen das lesen und wiederfinden eines bestimmten Codes um einiges leichter

2. magical values - beim testen ist es einfach zu vergessen eine genaue
 Beschreibung von einem Value, bzw eine Kennzeichnung, vergiss es also dann nicht auch danach.

3. magical strings - gleiche wie magical values, nur strings statt values

4. zu lange Methoden -  bei langen Methoden, kann es schnell dazu kommen, dass man verwirrt wird, was diese nun eigentlich macht.

5. falsche Benennungen - wenn schon ein Name vorhanden ist, was er sein sollte, sollte dieser auch sagen, was der Code tut

6. one Thing, one Method - lasse jeder Methode auch nur einen Job erledigen

7. einheitliche Benennung - wechsel nicht zwischen verschiedenen Benennungstilen. Halte dich am besten nach den Standarts

8. Testcode - vergiss nicht Code, der zum testen war, oder nicht mehr benützt wird zu löschen

9. Faule Klasse - wenn du eine Klasse machst, lass sie auch etwas erledigen

10. Datenklasse - Klassen mit Feldern ohne Funktionalität
