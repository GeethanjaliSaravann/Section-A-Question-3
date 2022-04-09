#include <bits/stdc++.h>
using namespace std;
int main ()
{
  char str1[100],str2[100];
  char temp;
    int i, j,len,n;
  cout<<"Enter the number of string to be entered = ";
  cin>>n;
  cout<<"Enter the string1 : ";
  cin>>str1;
  cout<<"Enter the string2 : ";
  cin>>str2;
  len = strlen(str1);
    for (i = 0; i < len-1; i++) {
        for (j = i+1; j < len; j++) {
            if (str1[i]< str1[j]) {
                    temp = str1[j];
                    str1[j] = str1[i];
                    str1[i] = temp;
            }
        }
    }
    cout<<"String1 :"<< str1;
    len = strlen(str2);
    for (i = 0; i < len-1; i++) {
        for (j = i+1; j < len; j++) {
            if (str2[i]< str2[j]) {
                    temp = str2[j];
                    str2[j] = str2[i];
                    str2[i] = temp;
            }
        }
    }
    cout<<"\nString2 :"<< str2;
    return 0;
}
