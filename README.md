# Nadra-identification-system-
//CS101 PROJECT-NADRA IDENTIFICATION SYSTEM
// OMAN SAID-2023575
// M.JUNAID RAZA-2023313
//M.AMMAR ALI-2023166
#include <iostream>
#include <string.h>
using namespace std;

int func();
int main()
{
    
	char choice;

    cout << "\nWelcome to NADRA's BioData section.\n";
    cout << "Would you like to proceed this section?\n";

    cout << "1.YES (Y)" << endl <<"2.NO (N)" << endl;
    cin >> choice;

    if (choice == 'Y' || choice == 'y'){
    	
		func();
    }
    
	cout<< "\n\n\t Thank You for using our website\n"<<"\t\tHave a good day!";
	return 0;
}
