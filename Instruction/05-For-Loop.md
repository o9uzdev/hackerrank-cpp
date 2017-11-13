# For Loop

https://www.hackerrank.com/challenges/c-tutorial-for-loop

```cpp
#include <iostream>
#include <cstdio>
using namespace std;

int main() {
    int a, b;
    int n = 0;
    string intMap[9]= { "one", "two","three","four","five","six","seven","eight","nine" };
    
    cin >> a >> b;
    
    if (( a <= 9) && ( b <= 9 )) { 
        for( n=a; n <= b; n++ ) {
            cout << intMap[n-1] << endl; 
        } 
    }

    else if (( a <= 9) && ( b>9 )) {    

        for( n=a; n <= 9; n++ ) {
            cout << intMap[n-1] << endl;
        }

        for( n=10; n <= b; n++ ) {    
            if ( n%2 == 0) {
                cout << "even" << endl;
            }
            else {
                cout << "odd" << endl;
            }
        }
    }

    return 0;
}
```