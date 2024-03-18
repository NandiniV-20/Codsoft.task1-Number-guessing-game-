#include<iostream>
#include<cstdlib>
using namespace std;

int main() {
    
    int randomNumber = rand() % 100 + 1; 
    cout << "***** WELCOME TO THE NUMBER GUSSING GAME! *****" << endl;
    cout << "\nI've selected a random number between 1 to 100. So,Guess the number!" << endl;
    
    int guess;
    do {
        cout << "Enter your guessed number: ";
        cin >> guess;
        
        if (guess < randomNumber){
            cout << "\nToo low! Try again." << endl;
        }
        else if (guess > randomNumber){
            cout << "\nToo high! Try again." << endl;
        }
        else{
            cout << "\n\tCongratulations! You've guessed the correct number. " << endl;
            cout<<"\n\n\t\tYOU WON THE GAME!!!";
        }
    } while (guess != randomNumber);
    
    return 0;
}
