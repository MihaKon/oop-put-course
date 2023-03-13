# This directory contains solution to the lesson-02


#include <iostream>

using namespace std;

class PersonalComputer {
	public: 
		string mobo;
		string cpu;
		string disk;
		int benchmarkSciore;
};

class Door{
public:
	bool isOpen;
private:
	bool isMonster;

public:
	void openDoor() {
		if (isOpen) {
			cout << "Door already opened\n";
			isOpen = true;
		}
		else {
			cout << "You open the door\n";
		}
	}
};


int main()
{
	PersonalComputer home;
	home.mobo = "TUF GAMING B550-PLUS";
	home.cpu = "i5-7500";
	home.disk = "toshiba";
	home.benchmarkSciore = -5;
    
	Door livingroom;
	livingroom.isOpen = false;

	char wouldHe;

	cout << "Mother Booard: " << home.mobo << "\n";
	cout << "Processor: " << home.cpu << "\n";
	cout << "Hard Drive: " << home.disk << "\n";
	cout << "Catzilla Score: " << home.benchmarkSciore << "\n";
	cout << "\n";
	cout << "####DOOR####\n";
	cout << "THE VIDEO GAME\n";
	cout << "\n";
	cout << "Would you like to open the DOOR?[Y/N]\n";
	cin >> wouldHe;
	if (wouldHe == 'Y') {
		livingroom.openDoor();
	}
}
