# PVA2 - Programování a vývoj aplikací
## Cvičení 15: GUI Tkinter

### 1
Vytvořte okno o velikosti  500x500 bodů. Název okna `Tlačítko` a umístěte na něj tlačítko.
Po zmáčknutí na tlačítko se okno uzavře.
Druhé tlačítko otevře dialogové okno se zprávou Ahoj

### 2
V okně zobrazte vstupní registrační formulář uživatele. Uživatel bude vyplňovat pole:
* jméno
* příjmení
* email

Po odeslání zobrazíte zadané údaje. 

### 3

Za využití efektivních metod nakreslete vlajku Řecka a Izraele.


### 4
Naprogramujte kalkulačku. Kalkulačku budete ovládat přes tlačítka. Výraz a výsledek se bude zobrazovat v textovém poli.

Nápověda:

```
# funkce eval vyhodnotí výraz
# a funkce str převede výsledek na řetězec
total = str(eval(expression))
```

```
# StringVar() je třída proměnných
# vytvoříme instanci této třídy
equation = StringVar()

# Vytvoření textového pole pro zobrazení výrazu
expression_field = Entry(gui, textvariable=equation)
```


Tlačítko s hodnotou a operací
```
# Ovládací tlačítka a jejich umístění do mřížky
button1 = Button(gui, text=' 1 ',
              command=lambda: press(1), height=1, width=7)
button1.grid(row=2, column=0)
```

Vyhodnocení
```
equal = Button(gui, text=' = ', fg='black', bg='red',
             command=equalpress, height=1, width=7)
equal.grid(row=6, column=3)
```
