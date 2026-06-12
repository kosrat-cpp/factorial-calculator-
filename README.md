# factorial-calculator-
A C++ program to find the factorial of a number and display its expansion of factorial.
#include <iostream>
using namespace std;

#include <iostream>
using namespace std;

// Find factorial using recursion

int factorial(int n)
{
    if(n <= 1) return 1;
    else return n * factorial(n - 1);
}

int main()
{
    int number;
    cout << "Enter a number to find its factorial" << endl;
    cin >> number;
    cout << endl;

    cout << "The expansion of " << number << " factorial is : ";
    
    for(int i = 1; i <= number; i++) {
        cout << i;
        if(i < number) {
            cout << " * ";
        } else {
            cout << " = ";
        }
    }
    cout << endl;
    
    cout << "The result of " << number << " is : " << factorial(number) << endl;

    return 0;
}



