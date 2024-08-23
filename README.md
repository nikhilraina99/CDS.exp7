## Experiment 7
# Aim
To create and perform basic operations on arrays and strings in C++.

# Software Used
- VS Code

# Problem Statements:

1. **Create an Array**
   - Write a C++ program to define and initialize an array.

2. **Reverse Array Elements**
   - Write a C++ program to reverse the order of elements in an array.

3. **Sum and Average of Array Elements**
   - Write a C++ program to compute the sum and average of elements in an array.

4. **Find Maximum and Minimum Elements**
   - Write a C++ program to find the maximum and minimum values in an array.

5. **Search for Element and Count Occurrences**
   - Write a C++ program to find the position of an element and count its occurrences in an array.

6. **Input from User**
   - Write a C++ program to take user input for various operations.

7. **String Concatenation**
   - Write a C++ program to concatenate two strings.

8. **Reverse a String**
   - Write a C++ program to reverse a string.

9. **Check for Palindrome**
   - Write a C++ program to check if a string is a palindrome.

# Theory

**Arrays:** In C++, an array is a data structure that stores multiple values of the same data type in contiguous memory locations. Arrays are useful for organizing data and performing operations on multiple elements simultaneously.

**Strings:** In C++, strings are sequences of characters. They can be represented using either the std::string class or C-style character arrays. Strings are used for storing and manipulating text data effectively.

# Program Codes:

```javascript
// Nikhil
// 23070123093
#include<iostream>
using namespace std;
int main()
{
    int n, i, j;
    cout << "Enter number of elements-";
    cin >> n;
    int a[n];
    cout << "Enter array elements-";
    for ( int i =0; i <n ; i++ )
    { cin >> a[i];
     
    }
       for (int i: a)
     {
        cout << " "<< i ;
     } 
    return 0;
}
```
```javascript
// Nikhil
// 23070123093
#include<iostream>
using namespace std;
int main()
{
     int n, i, j;
     float avg, s = 0;
cout << "Enter the number of elements: ";
cin >> n;
int a[n];
cout << "Enter array elements: ";
for( i = 0; i<n ; i++)
{
    cin >> a[i];
}

for (j= 0 ; j<n; j++)
{
    s = a[j]+s;
}
avg = s/n;
cout << "The sum of elements of the givne array is: "<<s<<endl;
cout << "The average of the given array is: "<< avg<<endl;

return 0;
}
```
```javascript
// Nikhil 
// 23070123093
#include<iostream>
using namespace std;
int main() 
{
    string name("Nikhil");
    string surname("Raina");
    name.append(surname);
    cout<<name<<endl;
}

// Nikhil
// 23070123093
#include<iostream>
using namespace std;
int main()
{
     int n, i, j, max, min;
cout << "Enter the number of elements: ";
cin >> n;
int a[n];
cout << "Enter array elements: ";
for( i = 0; i<n ; i++)
{
    cin >> a[i];
}
max = a[0];
min = a[0];
for (j= 1 ; j<n; j++)
{
 if (max<a[j])

 {
    max = a [j];
 }
 if (min > a[j])
 {
    min = a[j];
 }
}
cout <<"The maximum element in the given array is: "<<max<<endl;
cout << "The minimun element in the array is: "<<min<<endl;
return 0;

}
```
```javascript
// Nikhil 
// 23070123093
#include<iostream>
#include<string>
#include<algorithm>
using namespace std;
int main() 
{
    string s1, s2;
    cout << "Enter a word to check";
    cin>>s1;
    s2=s1;
    reverse(s1.begin(), s1.end());
    if (s2==s1) 
    {
        cout<<"Yes! It is a palindrome";
    }
    else cout<<"No! It is not a palindrome";
}
```
```javascript
// Nikhil
// 23070123093
#include<iostream>
using namespace std;
int main()
{
    int n, i, j;
    cout << "Enter number of elements ";
    cin >> n;
    int a[n];
    cout << " Enter array elements ";
    for ( int i=0; i<n ; i++ )
    { cin >> a[i];
     
    }
       for (j = n-1 ; j>=0; j--)
     {
        cout << " "<< a[j];
     } 
    return 0;
}
```
```javascript
// Nikhil
// 23070123093
#include<iostream>
#include<string>
#include<algorithm>
using namespace std;
int main()
{
    string a= "Nikhil";
    reverse(a.begin(), a.end());
    cout<<"reverse string is:"<<a<<endl;
    return 0;
    }
```
```javascript
// Nikhil
// 23070123093
#include<iostream>
using namespace std;
int main()
{
     int n, i, j, s, c = 0, flag = 0;
cout << "Enter the number of elements: ";
cin >> n;
int a[n];
cout << "Enter array elements: ";
for( i = 0; i<n ; i++)
{
    cin >> a[i];
}
cout << "Enter an element to be searched in an array: ";
    cin >> s;
for (j= 0 ; j<n; j++)
{
    if ( a[j]==s)
    {
cout<< "The element"<<" "<< s<< " " << "is present at location: "<<j<<endl;
c++;
flag =1;
    }
}

if( flag ==0)
{
    cout<< "The element"<< " "<< s << " "<< "is not present in the given array";
}
else
{
    cout << "The element" << " "<< s << " "<< "occurs"<< " "<< c << " "<< "times.";
}
return 0;
}
```
```javascript
// Nikhil
// 23070123093
#include <iostream>
using namespace std;
int main()
{
    char s[]= "Nikhil";
    cout<<s<<endl;
    return 0;
}
```
# Outputs:
1.

![Screenshot 2024-08-23 094726](https://github.com/user-attachments/assets/2fba8144-da6c-4454-babf-f0ded2cc2231)

2.

![Screenshot 2024-08-23 095001](https://github.com/user-attachments/assets/6ac96618-b58a-463f-9473-15987b4ce652)

3.

![Screenshot 2024-08-23 095341](https://github.com/user-attachments/assets/e6d933b2-29bb-4500-a49a-72b977a2861e)

4.

![Screenshot 2024-08-23 095728](https://github.com/user-attachments/assets/50f90871-3a8b-4238-bd0d-d49e2e025b3c)

5.

![Screenshot 2024-08-23 100116](https://github.com/user-attachments/assets/4acc45a5-a5c2-4970-81fc-2b38de8bbd5e)

6.

![Screenshot 2024-08-23 094441](https://github.com/user-attachments/assets/170d36a5-5dee-445d-8b0e-54414bd6f657)

7.

![Screenshot 2024-08-23 100242](https://github.com/user-attachments/assets/1ad64ccf-13c2-49ff-9ecd-8dbd2e6c7173)

8.

![Screenshot 2024-08-23 100505](https://github.com/user-attachments/assets/16812bac-45c1-46ee-9d6b-d41dbff878a5)

9.

![Screenshot 2024-08-23 100649](https://github.com/user-attachments/assets/c0b68d42-d4db-48a2-b1cf-86a026b48265)

# Conclusion:
- We learned how to create and work with arrays, including tasks such as reversing the order of elements, calculating the total sum, and identifying the maximum and minimum values.
- Additionally, we covered techniques for searching for specific elements, counting their occurrences, and performing various string operations like concatenation, reversing strings, and checking if a string is a palindrome.







