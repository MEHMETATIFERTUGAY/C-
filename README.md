# C-
#include <iostream>
using namespace std;

class Insan {
public:
    string isim;
    int yas;
    void isimveyassoyle() {
        cout << isim << " " << yas << endl;
    }

};
int main()
{
    Insan insan1,insan2;
    insan1.isim = "kaan";
    insan1.yas = 25;
    insan2.isim = "fatih";
    insan2.yas = 30;
    insan1.isimveyassoyle();
    insan2.isimveyassoyle();
    return 0;
}
