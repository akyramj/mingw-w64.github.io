#include<iostream>
using namespace std;
int main() {
	//Variabeln
	int Gesamtzahl, Volle_Boxen, Rest;
	int Ein_Box = 50;
	double Box_Preis = 4.50;
	double Schraube_Preis = 0.10;
	double Viele_Schrauben_Preis;
	double Viele_Boxen_Preis;
	double Gesamt_Preis;
	//Eingabe
	cout << "--- BauMax Verpackungs-Rechner ---" << endl;
	cout << "Bitte geben Sie die Gesamtanzahl der Schrauben ein: ";
	cin >> Gesamtzahl;
	cout << "" << endl;
	
	//Ausgabe
	cout << "--- Berechnung ---" << endl;
	Volle_Boxen = Gesamtzahl / Ein_Box;
	cout << "Volle Boxen (a 50 Stueck): " << Volle_Boxen << endl;
	Rest = Gesamtzahl - Volle_Boxen * Ein_Box;
	cout << "Lose Schrauben (Rest): " << Rest << endl;
	cout << "--- Preis ---" << endl;
	Viele_Boxen_Preis = Box_Preis * Volle_Boxen;
	cout << "Preis fuer" << Volle_Boxen << "Boxen: " << Viele_Boxen_Preis << " €" << endl;

	Viele_Schrauben_Preis = Schraube_Preis * 27;
	cout << "Preis fuer 27 Schrauben: " << Viele_Schrauben_Preis << " €" << endl;
	cout << "-------------------------" << endl;
	Gesamt_Preis = Viele_Schrauben_Preis + Viele_Boxen_Preis;
	cout << "Gesamtpreis: " << Gesamt_Preis << " €";

	return 0;


	



}
