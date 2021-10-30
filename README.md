# Lecture-9-2-
Reverse 9 times

    #include <iostream>
    using namespace std;

    int main()
    {
        int num = 108;
        while (num >= 9){
            cout << num << endl;
            num = num - 9;
        }
        cin.get();

        return 0;
    }
Pointless box

    #include <iostream> 
    using namespace std;
    int main()
    {
        cout << "This is a useless contraption. 1 or 2? \n";
        int num;
        cin >> num;

        while (num == 1 || num == 2) {
            cin.clear();
            if (num = 1) {
                cout << "Yes this is a 1. \n";
                cout << "This is useless. 1 or 2? \n";
                cin >> num;
            }
            else if (num = 2) {
                cout << "Yes this is a 2. \n ";
                cout << "This is useless. 1 or 2? \n";
                cin >> num;
            }
        }
        cout << "Invalid Input.";
    }
Pointless box endless loop

    #include <iostream>
    using namespace std;
    int main()
    {
        cout << "Enter a number either 1 or 2\n";
        string x;
        cin >> x;
        while (true)
        {
            if (x == "1")
            {
                cout << "you have entered the number 1\n";
                cout << "Enter a number either 1 or 2\n";
                cin >> x;
            }
            else if (x == "2")
            {
                cout << "you have entered the number 2\n";
                cout << "Enter a number either 1 or 2\n";
                cin >> x;
            }

            else
            {
                cout << "you did not enter the number 1 and 2\n";
                cout << "Enter a number either 1 or 2\n";
                cin >> x;
            }


        }


    }
Input imporvement

    #include <iostream> 
    using namespace std;
    int main() {
        char input;
        do {
            cout << "Would you like to Quit (Y/N)?" << endl;
            cin >> input;
        } while ((input != 'Y') && (input != 'y')); 



        return 0;
    }
Loopy
    
       #include <iostream>  
    using namespace std;
    int main() {

        int myInt = 0, counter;
        cout << "Enter a number\n";
        cin >> counter;
        do
        {
            cout << myInt << endl;
            myInt++;

        } while (myInt <= counter);

    }
Brute force I

    #include <iostream>
    using namespace std;
    int main()
    {
        string password = "246";
        string userInput;



        while (userInput != password)
        {
            cout << "Enter the pass code for the safe" << endl;
            cin >> userInput;

        }
        //to print the ran out of message only if the password was not found within 5 attempts
        cout << "You found the code";
    }
Brute force II

    #include <iostream>
    using namespace std;
    int main()
    {
        string password = "246";
        string userInput;
        int x = 5;
        cout << "You will only have 5 attempts" << endl;


        while (x > 0)
        {
            cout << "Enter the pass code for the safe" << endl;
            cin >> userInput;
            if (userInput == password)
            {
                cout << "You have finally unlocked the safe" << endl;

                break;
            }
            else
                x--;
        }
        //to print the ran out of message only if the password was not found within 5 attempts
        if (x == 0)
        {
            cout << "You ran out of attempts" << endl;
        }
    }




