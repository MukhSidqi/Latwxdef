#include <cstdlib>
#include <iostream>
#include <cmath>
using namespace std;

int main ()
{
    int a,b,c;
    float x1,x2,d;
    cout << "Masukan nilai a : " ;
    cin >> a;
    cout << "Masukan nilai b : " ;
    cin >> b;
    cout << "Masukan nilai c : " ;
    cin >> c;
    
    //hitung nilai determinan
    d = b*b - (4*a*c);
    
if (d>0)  {
       //menghitung nilai x1 dan x2
       x1 = (b + sqrt(d))/(2*a);
       x2 = (b - sqrt(d))/(2*a);
       
       //menampilkan nilai akar
       cout << "Akar x1 = " << x1 << endl;
       cout << "Akar x2 = " << x2 << endl;
          
}
else if (d == 0){
    //menghitung nilai x1 dan x2
    x1 = b /(2*a);
    x2 = x1;
    
    //menampilkan nilai akar kembar
    cout << "persamaan memiliki akar kembar" << endl;
    cout << "Akar x1 = x2 = " << x1 << endl;
}
else {
  //menampilkan pesan akar imaginer
  cout << "Akar x1 adalah bilangan imaginer" << endl;
  cout << "Akar x2 adalah bilangan imaginer" << endl;
}

  system ("PAUSE");
  return 0;
}
  
    

 
