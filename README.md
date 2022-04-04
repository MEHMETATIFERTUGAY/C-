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
#include <iostream>
#include "hayvan.h"


using namespace std;
int main()
{
	hayvan hayvan1;
	hayvan1.isim = "pamuk";
	hayvan1.sinif = "kedi";
	hayvan1.tur = "british";
	hayvan1.yas = 1;
	hayvan1.ozelliklerinisoyle();
	return 0;
}
    #include"hayvan.h"
#include <iostream>

void hayvan::ozelliklerinisoyle() {
	cout << hayvan::isim << " " << hayvan::sinif << " " << hayvan::tur << " " << hayvan::yas << endl;

}

    #include <string>
using namespace std;
class hayvan {
public:
	string isim;
	string tur;
	string sinif;
	int yas;

	void ozelliklerinisoyle();
};
