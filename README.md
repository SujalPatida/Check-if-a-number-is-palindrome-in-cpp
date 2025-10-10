#include <iostream>
using namespace std;

int main() {
    int num, original, reversed = 0;

    cout << "Enter a number: ";
    cin >> num;

    original = num;  // Store the original number

    while (num != 0) {
        int digit = num % 10;            // Get the last digit
        reversed = reversed * 10 + digit; // Build the reversed number
        num = num / 10;                  // Remove the last digit
    }

    if (original == reversed)
        cout << original << " is a Palindrome number." << endl;
    else
        cout << original << " is NOT a Palindrome number." << endl;

    return 0;
}
