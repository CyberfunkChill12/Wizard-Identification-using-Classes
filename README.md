# Wizard-Identification-using-Classes

#include <iostream>

using namespace std;

//Create your class Wizard here.
class Wizard {
    private:
        int wizardAge;
        string wizardtitle1;
        int wizard_ID;
        string wizardLast1;
    public:
        void set_wizardAge (int a){
            wizardAge = a;
        }
        void set_wizard_ID(int i){
            wizard_ID = i;
        }
        int get_wizardAge () {
            return wizardAge;
        }
        void set_wizardFirstName (string wizardName){
            wizardtitle1 = wizardName;
        }
        int get_wizard_ID () {
            return wizard_ID;
        }
        string get_wizardFirstName (){
            return wizardtitle1;
        }
        string get_wizardLastName () {
            return wizardLast1;
        }
        void set_wizardLastName (string wizardLast) {
            wizardLast1 = wizardLast;
        }
};
int main() {
//DO NOT MODIFY THE MAIN()!!!!
    int wizardAge, wizard_ID;
    string wizardFirstName, wizardLastName;
    
    cin >> wizardAge >> wizardFirstName >> wizardLastName >> wizard_ID;
    
    Wizard wiz;
    wiz.set_wizardAge(wizardAge);
    wiz.set_wizard_ID(wizard_ID);
    wiz.set_wizardFirstName(wizardFirstName);
    wiz.set_wizardLastName(wizardLastName);
    
    cout << wiz.get_wizardAge() << "\n";
    cout << wiz.get_wizardLastName() << ", " << wiz.get_wizardFirstName() << "\n";
    cout << wiz.get_wizard_ID();
    
    return 0;
}
