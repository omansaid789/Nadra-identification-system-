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
       case '4':
							cout << "Division of "  << name << " is:\tKohat\n";
							switch (CNICnum[2])
				                        	{
					                        	case '1':
							                        cout << "District of "  << name << " is:\tKohat\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tHangu\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tHangu\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tTal\n";
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
							                        cout << "District of "  << name << " is:\tKohat\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tKarak\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tBanda Daud Shah\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tKarak\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tTakht Nusrati\n";
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
							                        cout << "District of "  << name << " is:\tKohat\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tKohat\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tKohat\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tLaachi\n";
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
						case '5':
							cout << "Division of "  << name << " is:\tMalakand\n";
							switch (CNICnum[2])
				                        	{
					                        	case '0':
							                        cout << "District of "  << name << " is:\tDeer\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tDeer\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '0':
						                                        	cout << "Union Council of "  << name << " is:\tDeer\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                        case '1':
							                        cout << "District of "  << name << " is:\tBuner\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tBuner\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tDagar\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tGagarah\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tTotalaye\n";
							                                    break;
							                                    case '4':
						                                        	cout << "Union Council of "  << name << " is:\tMandnarh\n";
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
							                        cout << "District of "  << name << " is:\tLower Chitral\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tLower Chitral\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tChitral\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tMastuj\n";
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
							                        cout << "District of "  << name << " is:\tLower Dir\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tLower Dir\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tKhall\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tTemargara\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tSamar Bagh\n";
							                                    break;
							                                    case '4':
						                                        	cout << "Union Council of "  << name << " is:\tMunda\n";
							                                    break;
							                                    case '5':
						                                        	cout << "Union Council of "  << name << " is:\tLal Qila\n";
							                                    break;
							                                    case '6':
						                                        	cout << "Union Council of "  << name << " is:\tBalambat\n";
							                                    break;
							                                    case '7':
						                                        	cout << "Union Council of "  << name << " is:\tAudn Zai\n";
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
							                        cout << "District of "  << name << " is:\tMalakand\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tMalakand\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tDargai\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tBatkhela\n";
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
							                        cout << "District of "  << name << " is:\tShangla\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tShangla\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tAlpuri\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tBashaam\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tChakesar\n";
							                                    break;
							                                    case '4':
						                                        	cout << "Union Council of "  << name << " is:\tMartoang\n";
							                                    break;
							                                    case '5':
						                                        	cout << "Union Council of "  << name << " is:\tPuran\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                        case '6':
							                        cout << "District of "  << name << " is:\tSwat\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tSwat\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tMatt\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tMingora\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tBrekot\n";
							                                    break;
							                                    case '4':
						                                        	cout << "Union Council of "  << name << " is:\tKabl\n";
							                                    break;
							                                    case '5':
						                                        	cout << "Union Council of "  << name << " is:\tKhawaza Khaila\n";
							                                    break;
							                                    case '6':
						                                        	cout << "Union Council of "  << name << " is:\tCharbagh\n";
							                                    break;
							                                    case '7':
						                                        	cout << "Union Council of "  << name << " is:\tBabu Zai\n";
							                                    break;
							                                default:
				                                            cout << "The entered CNIC has an invalid union council number\n";
		                                               	}
							                            break;
							                        default:
							                        cout << "The entered CNIC number has an invalid Tehsil number\n";
				                                 	}
						                        	break;
						                        case '7':
							                        cout << "District of "  << name << " is:\tShangla\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tUpper Dir\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tRohan\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tWarhi\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tKalkot\n";
							                                    break;
							                                    case '4':
						                                        	cout << "Union Council of "  << name << " is:\tBrawal\n";
							                                    break;
							                                    case '5':
						                                        	cout << "Union Council of "  << name << " is:\tKhal\n";
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
                        case '6':
							cout << "Division of "  << name << " is:\tMardan\n";
							                    switch (CNICnum[2])
				                        	{
					                        	case '1':
							                        cout << "District of "  << name << " is:\tMardan\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tMardan\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tMardan\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tTakht Bhai\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tKatlang\n";
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
							                        cout << "District of "  << name << " is:\tSwabi\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tRazzar\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tLahor\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tswabi\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tTopi\n";
							                                    break;
							                                    case '4':
						                                        	cout << "Union Council of "  << name << " is:\tK.S.K\n";
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
                        case '7':
							cout << "Division of "  << name << " is:\tPeshawar\n";
							switch (CNICnum[2])
				                        	{
					                        	case '1':
							                        cout << "District of "  << name << " is:\tCharsadda\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tCharsadda\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tCharsadda\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tTangi\n";
							                                    break;
							                                    case '3':
						                                        	cout << "Union Council of "  << name << " is:\tShahqadar\n";
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
							                        cout << "District of "  << name << " is:\tNowshera\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tNowshera\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tNowshera\n";
							                                    break;
							                                    case '2':
						                                        	cout << "Union Council of "  << name << " is:\tPabbi\n";
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
							                        cout << "District of "  << name << " is:\tPeshawar\n";
							                        switch (CNICnum[3])
					                                {
						                                case '0':
						                                	cout << "Tehsil of "  << name << " is:\tPeshawar\n";
						                                	switch (CNICnum[4])
					                                        {
					                                        	case '1':
						                                        	cout << "Union Council of "  << name << " is:\tKhail\n";
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
                          
						default:
							cout << "The entered CNIC number has an invalid Division number\n";
					}
				break;
							default:
				cout << "The entered CNIC has an invalid province number\n";
			}

			cout << "Family tree of "  << name << " is:\t" << CNICnum[5] << CNICnum[6] << CNICnum[7] << CNICnum[8] << CNICnum[9] << CNICnum[10] << CNICnum[11];
	return 0;
}
