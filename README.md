# Find-the-number-that-appear-once-and-the-others-appear-twice
#include <bits/stdc++.h>

using namespace std;
 
int getsingleElement(vector<int> &arr){
    int n = arr.size();
    int xorr = 0;
    for(int i=0; i<n; i++){
        xorr = xorr ^ arr[i];
    }
    return xorr;
}

int main(){
    vector<int> arr = {4,1,2,1,2};
    int ans = getsingleElement(arr);
    cout<< " single element is  "<< ans <<endl;
    return 0;
}
