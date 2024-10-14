
# Number Guessing Flowchart!!!!
yay!

``` mermaid
    flowchart TD
    A([X becoms a rand num 1-10]) --> B{User then is prompted to give guess Y or quit, User is also told range of numbers}
    B --> a(Y < X)
    B --> b(Y > X)
    B --> c(Y = X)
    B --> d[/Quit/]
    B --> e(Y is not a valid answer, not a number)
    B --> f(Y > 10 or Y < 1)
    a --> Ca[\Too low!\]
    Ca --> B
    b --> Cb[\Too High!\]
    Cb --> B
    c --> Cc[\Hooray!!\]
    d --> Cd([App Closes])
    e --> Ce[\Not valid answer\]
    Ce --> B
    f --> Cf[\Remember! The number is 1-10\]
    Cf --> B
    Cc --> D[\Try Again?\]
    D --> Da[/Y/]
    D --> Db[/N/]
    Da --> A
    Db --> Cd
```