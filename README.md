# Sorting-an-array-in-ascending-order

#include <bits/stdc++.h>
 using namespace std;
 int main()
{

    int x;
    cin>>x;
    int arr[x];
    for(int i = 0;i<x;i++)cin>>arr[i];
    sort(arr,arr+x);
    for(int i = 0;i<x;i++)cout<<arr[i]<<" ";
    return 0;
    
}



#include <iostream>
using namespace std;
int main()
{


    int n,i,j,m;
    cin>>n;
    int a[n];
    for(i=0;i<n;i++)
    {
        cin>>a[i];
    }



    for(i=0;i<n;i++)
    {
        for(j=i+1;j<n;j++)
        {
            if( a[i] > a[j] )
            {
                m=a[j] ; a[j] = a[i]; a[i]=m;
            }
        }

    }

    for(i=0;i<n;i++)
    {
        cout<<a[i] << " " ;
    }
    return 0;
}
