# Recupera-o
minha recuperação de TP
#include <iostream>
#include <vector>
using namespace std;
 
int main()
{
  float lat;
  vector<float> lista;
  cout << "Escreva um valor maior que 1 para começar: ";
  cin >> lat;
  float typed = lat+1;
  
  while(typed > lat)
  {
  lat = typed;
  cout << "Escreva um valor maior que o anterior (" << lat << ") : ";
  cin >> typed;
  lista.push_back(typed);
  for (size_t i = 0; i < lista.size();i++)
    {
    cout << lista[i];
    }
  cout << endl;
  }
  cout << "Error 404! Você escreveu um valor menor ou igual que o anterior!";
}
