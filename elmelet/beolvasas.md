# Beolvasas

## Beolvasas billentyuzetrol

```c++
#include <iostream>

int x;
cin >> x; // beolvas egy int szamot

char s[100];
cin.getline(s, 100); // beolvas enterig vagy a 100 hosszusagig
cin >> s; // beolvas space-ig

char c;
cin >> c; // beolvas egy karaktert

```

## Beolvasas fajlbol

```c++
#include <fstream>

ifstream f("be.txt"); // iez felelos a beolvasasert

ofstream g("ki.txt"); // ez felelos a kiirasert


char s[100], c;
f>> s; // beolvas egy szot (space-ig)
f.getline(s, 100); // beolvas egy sort (entereig vagy addig amig a 100 hosszusagot el nem eri)
f>> c; // beolvas egy karaktert

// addig amig el nem eri a fail veget
while(!f.eof()){
    f>> s;
    //csinlunk valamit
}
// !!VIGYAZAT ez egyel tobbet olvas be mint amit kell


//VAGY

while(f){ // ugyan az mint az elozo csak rovidebb
    f>> s;
    //csinlunk valamit

}

//VAGY AMIT EN AJANLOK:
while(f>>s){   // ameddig tud olvas ha nem akkor megall es nem olvas + ba
    //csinalunk valamit
}


```

## Kiiratas

```cpp

g<< "szoveg" << endl; // endl: uj sor

```

## Bezaras (ajanlott)

```cpp
f.close();
g.close();
```
