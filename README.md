# Summative-Assessment-2-Resubmission

    #include<iostream>
    #include<string>
    #include <math.h>
    using namespace std;
    int main()
    {
        string name;
        double n, p, f = 1, x = 1, cube, square;
        cout << "\n>>>>>>>>>>> FACTORIAL, TABLE FROM 20 - 30, SQUARE AND CUBE >>>>>>>>>>> \n";
        cout << "\n\nPlease enter your full name: ";
        getline(cin, name);
        cout << "\nFrom 1 - 10, Enter the number that you want to calculate: ";
        cin >> n;

        while (cin.fail())
        {
            cout << "\nInvalid Input\n\n";
            cout << "Enter the number again: ";
            cin.clear();
            cin.ignore(1000, '\n');
            cin >> n;
        }

        cout << "\n\n>>>>>>>>>>> FACTORIAL >>>>>>>>>>>>>>>>>>>>\n";
        do
        {
            f = f * x;
            x++;
        } 
        while (x <= n);
        cout << "\nFactorial of " << n << " is " << f << endl;

        cout << "\n\n>>>>>>>>>>> TABLE FROM 20 - 30 >>>>>>>>>>>\n\n";
        for (double i = 20; i <= 30; i++)
        {
            p = n * i;
            cout << n << " x " << i << " = " << p << endl;
        }

        cout << "\n\n>>>>>>>>>>> SQUARE AND CUBE >>>>>>>>>>>>>>\n";
        while (x <= n);
        {
            cube = cbrt(n);
            square = sqrt(n);

            cout << " \nThe Cube of " << n << " is: " << cube << endl;
            cout << "The Square of " << n << " is: " << square << endl;
        }

    }
