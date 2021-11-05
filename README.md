#include <iostream>

using namespace std;

int main ()
{
	int SecretNum = 7;
	int guess;
	int GuessCount = 0;
	int GuessLimit = 3;
	bool OutOfGuesses = false;
	
	while(SecretNum != guess)
		{
		if(GuessCount < GuessLimit)
			{
			cout << "Enter guess: ";
			cin >> guess;
			GuessCount++;
			}
		  else OutOfGuesses = true;
		}
		
	if(OutOfGuesses) cout << "You lose!";
	  else cout << "You win!";
	
	return 0;
}
