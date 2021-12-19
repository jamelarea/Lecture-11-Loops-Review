# Lecture-11-Loops-Review

SLIDE 3, Execute this code and see what’s the issue

    #include <iostream>
    using namespace std;

    int main()
    {
        int y;
        cout << "Enter a number you want the table of: ";
        cin >> y;
        while (cin.fail()) //returns true when an input failure occurs
        {
            cin.clear(); //clears the error flag on cin
            cin.ignore(1000, '\n'); //skips to the next newline
            cout << "Invalid command enter the number again: ";
            cin >> y;
        }
        for (int x = 0; x <= 10; x++)
        {   cout << y << "x" << x << "=" << y * x << endl;

        }
        return 0;
    }
    
SLIDE 4, Stars

    #include <iostream>
    using namespace std;
    
    int main()
    {
        int i = 1;
        int j = 1;
        while (i <= 5) {
            j = i;
            while (j <= 5) {
                cout << "*";
                j++;
            }
            cout << endl;
            i++;
        }
        return 0;
    }
    
SLIDE 5, Stars

    #include <iostream>
    using namespace std;
    
    int main()
    {
        int i = 0;
        while (i < 5) {
            int j = 0;
            while (j <= i) {
                cout << "*";
                j++;
            }
            cout << endl;
            i++;
        }
    }
    
SLIDE 6, Stars
    
    #include <iostream>
    using namespace std;
    
    int main()
    {
        int i = 1;
        int j = 1;
        while (i <= 5) {
            j = i;
            while (j <= 5) {
                cout << "*";
                j++;
            }
            cout << endl;
            i++;
        }
        int k = 0;
        while (k < 5) {
            int l = 0;
            while (l <= k) {
                cout << "*";
                l++;
            }
            cout << endl;
            k++;
        }
    }
    
SLIDE 7, Factorial
    
    #include <iostream>
    using namespace std;
    
    int main()
    {
        int n;
        double factorial = 1.0;

        cout << "Enter an integer: ";
        cin >> n;

        for (int i = 1; i <= n; ++i) {
            factorial *= i; //formula
        }
        cout << "Factorial of " << n << " is " << factorial << endl;
    }
    
SLIDE 8, Table (For Loop)
    
    #include <iostream>
    using namespace std;
    
    int main()
    {
        int num;

        cout << "Enter a number: ";
        cin >> num;

        for (int i = 1; i <= 10; i++) {
            cout << num << " * " << i << " = " << (i * num) << "\n";
        }
        cin >> num;
        return 0;
    }
    
SLIDE 9, Table (While Loop)

    #include <iostream>
    using namespace std;
    
    int main()
    {
        int x, y, z;
        y = 1;
        z = 10;

        cout << "Enter a number: ";
        cin >> x;

        while (y <= z) {
            cout << x << " * " << y << " = " << y * x << endl;
            y = y + 1;
        }
        return 0;
    }
    
SLIDE 10, Table (For Loop)

    #include <iostream>
    using namespace std;
    
    int main()
    {
        int num1, num2;

        cout << "Enter the number you want the table of: ";
        cin >> num1; //multiplicand
        cout << "Enter till what number the table should end: ";
        cin >> num2; //multiplier

        for (int i = 1; i <= num2; i++) {
            cout << num1 << " * " << i << " = " << (i * num1) << "\n"; //printing
        }
        return 0;
    }
    
SLIDE 11, Find the 9s (Do-While Loop)
    
    #include <iostream>
    using namespace std;

    int main()
    {
        //variables
        int sum = 0;
        int num = 100;

        cout << "The integers between 0 till 200 that are divisible by 9 are:" << endl; //character output

        do
        {
            if (num % 9 == 0) //number divisible by 9
            {
                cout << num << endl;
                sum = sum + num; //formula for total
            }
            num++;

        } while (num <= 200); //number until 200
        //character output
        cout << "\nThe sum of integers between 0 and 200 divisible by 9 is: " << sum << endl;

        return 0;
    }
    

    
