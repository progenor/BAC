# CHAR ARRAY CSTRING

## Cstring

```c++
#include <cstring>
```

ha a cstringet akarod hasznalni eloszoer be kell includeolni

## Deklaralas

```c++
char s[100]; // 100 hosszu char tomb
char *p; // pointer ami egy charra mutat


```

# Kinezet

egy char tombnek a vegen mindig van egy '\0' ami jelzi a string veget

## Beolvasas

```c++
char s[100];
cin >> s; // beolvas egy szot (space-ig)
cin.getline(s, 100); // beolvas egy sort (entereig vagy addig amig a 100 hosszusagot el nem eri)

char c;
cin >> c; // beolvas egy karaktert

```

## egy par alap fuggveny:

```c++
strlen() // visszaadja a string hosszat
strcpy() // masolja a stringet (amibe masolunk, amit masolunk) !!kitorli ami eddig volt benne
strcat() // osszefuzi a stringeket (amibe masolunk, amit masolunk) ! ramasolja a masodikat az elso vegere
strcmp() // osszehasonlit ket stringet
strchr() // megkeresi az elso elofordulast egy karakternek (amiben, amit)
strstr() // megkeresi az elso elofordulast egy stringnek (amiben, amit)
strtok() // szetvagja a stringet egy karakter szerint (amit szetvagunk, amivel szetvagunk)


```

## strtok hasznalata

```c++
char s[100] = "alma korte szilva";
char *p = strtok(s, " "); // elso hivasnal a stringet adom meg, a masodiknal NULL-t
while(p){
    cout << p << endl;


    p = strtok(NULL, " "); // a strtok mindig a stringet modositja, ezert kell a masodik hivasnal NULL-t adni
}
```

## Ramasolni egy egyeduli char-t egy char tombbe

```c++
char s[100] = "szia";
char c = 'a';

strcat(s, &c); // kell az & mert a strcat char* parametert var


```

## For ciklusos bejaras

```c++
char s[100] = "szia";
for(int i=0;i<strlen(s);i++){
    cout << s[i] << endl;
}
```

VAGY

```cpp
for(int i=0;s[i] != '\0';i++){
        cout << s[i] << endl;
}
```
