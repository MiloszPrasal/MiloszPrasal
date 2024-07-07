# MiloszPrasal
// Books




 
#include <iostream>

using namespace std;



struct ksiazka {
    char tytul[100];
    char autor[100];
    int rok;
};

 int main() {
    int n;
    int i;
    cout << "Jak duzo ksiazek masz w swojej bibliotece: " << endl;
    cin >> n;

  
   ksiazka ksiazki[i];

  
    for (int i = 0; i < n; ++i) {
        cout << "Podaj tytul ksiazki " << i + 1 << ": " << endl;
        cin.ignore();
        cin >> ksiazki[i].tytul;

        cout << "Podaj autora ksiazki " << i + 1 << ": " << endl;
        cin >> ksiazki[i].autor;

        cout << "Podaj rok wydania ksiazki " << i + 1 << ":" << endl;
    }

    cout << "Twoje wszystkie ksiazki:" << endl;
    for (int i = 0; i < n; ++i) {
        cout << "Tytul: " << ksiazki[i].tytul << ", Autor: " << ksiazki[i].autor << ", Rok produkcji: " << ksiazki[i].rok << endl;
    }
    int szukajksiazki(ksiazka ksiazki[], int n, const char* tytul) 
    {
    
    for (int i = 0; i < n; ++i) {
        int j = 0;
       
        while (ksiazki[i].tytul[j] != '1' && tytul[j] != '1') 
        {
            if (ksiazki[i].tytul[j] != tytul[j]) 
            {
                break; 
            }
            ++j;
        }
       
        if (ksiazki[i].tytul[j] == '1' && tytul[j] == '1') 
        {
            return i;
        }
    }
    }
    
}
