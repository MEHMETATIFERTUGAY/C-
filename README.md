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
	#include<iostream>
#include<string>
using namespace std;

class person {

	string name;
	string surname;
	int age;
public:
	person() {
		name = "nothing";
		surname = "nothing";
		age = 0;
	}
	person(string n, string s, int a) {
		name = a;
		surname = s;
		age = a;

	}
	void print() {
		cout << "name : " << name << "\nsurname : " << surname << "\nage : " << age;
	}

};
class family {
public:

	int number_of_children, kindergeld;

	person member;



	family() {
		number_of_children = 0;
		kindergeld = 0;

	}

	family(person m, int n) {
		member = m;
		number_of_children = n;
		 getkindergeld();

	}

	int getkindergeld() {
		if (number_of_children < 3) {
			kindergeld = number_of_children * 184;
		}
		else if (number_of_children == 3) {
			kindergeld = (number_of_children-1) * 184 + 190;
		}
		else if (number_of_children > 3 )  {
			kindergeld = 184 * 2 + 190 + (number_of_children - 3) * 215;
		}
		return kindergeld;
	}

	void printInfo() {
		member.print();
		cout << "number of childeren : " << number_of_children << " \nkindergel : " << kindergeld << endl;
	}
};
int main() {
	person defaultperson;
	person father("atif", "ertugay", 20);

	father.print();
	cout << endl;
	defaultperson.print();
	family Fam(father, 2);
	cout << "Print family information :" << endl;
	Fam.printInfo();
}


