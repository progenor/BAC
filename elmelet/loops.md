# LOOPOK fajtaji

## FOR loop

hasznos ha tudjuk meddig kell menni honnan indulunk es mennyivel lepunk minden egyes alkalommal

```cpp

for(honnen; meddig; mennyivel)

for(honnen1, honnen2; meddig1  or/and meddig2; mennyivel1, mennyivel2)


// elszamol 10 ig
for(int i=0;i<10;i++){
    cout << i << endl;
}


```

## WHILE loop

addig meg mig a feltetel igaz

!VIGYAZAT ne csinaljunk infinite loopot

```cpp

while(igazsagi ertek){
    //csinalunk valamit
}

```

## DO WHILE loop

ugyan olyan mint a sima while, annyiban mas, hogy ez csak akkor nez a feltetelre amikor mar egyszer lefutott

tehat 1szer igyis ugyis lefut es majd ha az ertek nem igaz akkor megall, mig a sima while loop csak akkor fut le ha az ertek igaz

```cpp
do{
    //csinalunk valamit
}while(igazsagi ertek); // ; ne felejtsuk el

```
