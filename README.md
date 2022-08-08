 DCIT-104-ASSIGNMENT
 
#include <iostream>
using namespace std;
 void prime(int y);
int main()
{
int m = 0;

    cout << "Any number : " <<endl;
    cin >> m ;
    prime(m);
    
}
 void prime (int y)
 {
   int sum = 0;
    for (int t = y ; t > 1  ; t--)
    {

    bool isPrime = true;
    for (int j = 2 ; j < t ; j++)
    {
        if(t % j == 0)
            {
            isPrime = false;
            j = t;
            }
    }
    if (isPrime == true)
        {
        cout << "prime number: " << t << " , " ;
        sum = sum + t;
        }
    }
    cout << endl<< "sum of the given prime numbers : " << sum ;



}
