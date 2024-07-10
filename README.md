
#include <iostream>
#include <string>

using namespace std;




    


 int main() 
 {
    int n;
    int i;
    cout << "Jak duzo ksiazek masz w swojej bibliotece: " << endl;
    cin >> n;
    
    string tytul[n];
    string autor[n];
    int rok;
  
   

  
    for (int i = 0; i < n; ++i) {
        cout << "Podaj tytul ksiazki " << i + 1 << ": " << endl;
       
        cin >> tytul[n];

        cout << "Podaj autora ksiazki " << i + 1 << ": " << endl;

        cin >> autor[n];

        cout << "Podaj rok wydania ksiazki " << i + 1 << ":" << endl;

        cin >> rok;
    }

    cout << "Twoje wszystkie ksiazki:" << endl;
    for (int i = 0; i < n; ++i) 
    {
        cout << "Tytul: " << tytul[n] << ", Autor: " << autor[n] << ", Rok produkcji: " << rok << endl;
    }
 }
   
