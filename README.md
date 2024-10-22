# Experiment-15

Aim:
To study and implement Recursion.

Theory:
In C++, recursion is executed through when a function calls itself. The concept itself is essentially the same as in other programming languages; the function ultimately calls itself with changed arguments consistently until a base case is reached at which point it will stop calling itself and begin returning results along the route of recursive calls.

Properties of Recursion:
→ Base Case: Recursion stops when there is a condition.
→ Recursive Case: It is a solution to sub problems through recursive call.
→ Call Stack: The modules that contain each separate function in memory.
→ Overhead: Non-direct calculations that bite into the call and storage space.
→ Memory Consumption: Excessive levels of recursion may lead to rampant overflow of state.
→ Tail Recursion: This is a type of recursion where the last action is that of invoking another instance of the same function, and thus optimizations can be made.
→ Direct/Indirect Recursion: This is an instance of recursion in which the function invokes itself directly or indirectly.
→ Multiple Recursive Calls: Functions can perform more than one recursive call.
→ Backtracking: This method is used in algorithms that use multiple paths to find solutions.

CODE:-

15a
```
#include <iostream>
using namespace std;
int add(int n)
{
    if (n<=1)
    {
        return 1;
    }
    else
    {
        return (n+add(n-1));
    }
}
int main()
{
    int x,n;
    cout<<"Enter a number: ";
    cin>>n;
    x= add(n);
    cout<<x;
}
```

15b
```
#include <iostream>
#include <string>
using namespace std;
void rev(char *str)
{
    if (*str)
    {
        rev(str+1);
        cout<<("%c",*str);

    }

}
int main()
{
    char s[50];
    cout<<"Enter a string: ";
    cin>>s;
    rev(s);
}
```



