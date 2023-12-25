# Nadra-identification-system-
//CS101 PROJECT-NADRA IDENTIFICATION SYSTEM
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
int func(){
	
	string name;
	
	string CNICnum;
    
	int check;
	
	string province;

	cout << "Enter Person's CNIC number: \n";
	cin  >> CNICnum;
	while(CNICnum.length()!=13){
		cout<<"Invalid CNIC number entered. Enter the number again. "<<endl;
		cin>>CNICnum;
	}
      
    cin.ignore();
    
	cout <<"\nEnter name of Person : \n";
	getline(cin,name);
	
	check = CNICnum[12] % 2;
    
    if (check == 0)                           
	{
		cout << "\nGender of "  << name << " is:   Female" << endl;
	}
	else
	{
		cout << "\nGender of "  << name << " is:   Male" << endl;
	}
		switch (CNICnum[0]) 
		{
			case '1':
				cout << "Province of "  << name << " is:\tKhyber Pakhtunkhwa\n";
					switch (CNICnum[1])
					{
						case '1':
							cout << "Division of "  << name << " is:\tBannu\n";
							                    switch (CNICnum[2])
				                        	{
					                        	case '1':
							                        cout << "District of "  << name << " is:\tBannu\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tBannu\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tBannu\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tDomail\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                        case '2':
							                        cout << "District of "  << name << " is:\tBannu Cantonment\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tBannu Cantonment\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tLucky Marwat\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tSarai Norang\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                    	default:
							                    cout << "The entered CNIC number has an invalid District number\n";
					                        }
							break;
						case '2':
							cout << "Division of "  << name << " is:\tDERA ISMAIL KHAN\n";
							switch (CNICnum[2])
				                        	{
					                        	case '1':
							                        cout << "District of "  << name << " is:\tDERA ISMAIL KHAN\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tDERA ISMAIL KHAN\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tDERA ISMAIL KHAN\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tKulachi\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tPaharpur\n";
							                                    break;
							                                    case '4':
						                                        	cout << "Union Council of "  << name << " is:\tDarabin\n";
							                                    break;
							                                    case '5':
						                                        	cout << "Union Council of "  << name << " is:\tPerwa\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                        case '2':
							                        cout << "District of "  << name << " is:\tTaank\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tTaank\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tTaank\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                    	default:
							                    cout << "The entered CNIC number has an invalid District number\n";
					                        }
							break;
       case '3':
							cout << "Division of "  << name << " is:\tHAZARA\n";
							switch (CNICnum[2])
				                        	{
					                        	case '1':
							                        cout << "District of "  << name << " is:\tAbottabad\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tHavelian\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tBanda\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tSeer Garhi\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                        case '2':
							                        cout << "District of "  << name << " is:\tBatagram\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tBatagram\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tElai\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tKooza Banda\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                        case '3':
							                        cout << "District of "  << name << " is:\tHaripur\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tHaripur\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tGhazi\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tKot Najeebullah\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                        case '4':
							                        cout << "District of "  << name << " is:\tKohistan\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tKohistan\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tDaso\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tKolaye Pals\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tPatan\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                        case '5':
							                        cout << "District of "  << name << " is:\tManshera\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tMansehra\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tBalakot\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tKala Dhaka\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tMansehra\n";
							                                    break;
							                                    case '4':
						                                        	cout << "Union Council of "  << name << " is:\tAugi\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                    	default:
							                    cout << "The entered CNIC number has an invalid District number\n";
					                        }
							break;
