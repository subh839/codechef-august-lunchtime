# codechef-august-lunchtime

KMAX2
->
#include <bits/stdc++.h>
using namespace std;

int main() {
	int t;
	cin>>t;
	while(t--){
	    long long n,m;
	    cin>>n>>m;
	    long long maxi=-1;
	    long long a[n];
	    for(int i=0;i<n;i++){
	        cin>>a[i];
	        maxi=max(maxi,a[i]);
	    }
	    long long ans=0;
	    for(int i=m-1;i<n;i++){
	        if(a[i]==maxi){
	            ans+=(n-i);
	        }
	    }
	    cout<<ans<<"\n";
	}
	return 0;
}

: MXEVNSUB

#include <bits/stdc++.h>
using namespace std;

int main() {
int t;
cin>>t;
while(t--){
    int n;
    cin>>n;
    if((n%4==0)||((n+1)%4==0))
    {
        cout<<n<<"\n";
    }
    else{
        cout<<n-1<<"\n";
    }
}
	return 0;
}



JAG
#include <bits/stdc++.h>
using namespace std;

int main() {
	int t;
	cin>>t;
	while(t--){
	    int n;
	    cin>>n;
	    int a[n];
	    map<int , int>mp;
	    int ans=0;
	    for(int i=0;i<n;i++){
	        cin>>a[i];
	        mp[a[i]-i-1]++;
	        if(mp[a[i]-i-1]==1){
	            ans++;
	        }
	    }
	    if(mp[a[0]-1]==n){
	        cout<<n<<"\n";
	    }
	    else{
	        cout<<1<<"\n";
	    }
	}
	return 0;
}



ucode->
q)Archie is very fond of ice creams. He went to an ice cream parlor to buy some ice creams.There are N containers which contain the ice creams. The i−th container has Ai ice creams.He has some rules. He will take ice creams from the containers in the following way:

Container with 10 or lesser ice creams, he does not take any.
Container with more than 10 ice creams,
he takes all ice-creams but leaves 10 ice creams. Your task is to find the total number of Ice creams Archie will take back home.
#include <iostream>
using namespace std;

int main() {
	int t;
	long long int sum=0;
	cin>>t;
	while(t--){
	    long long int n;
	    cin>>n;
	    long long int a[n];
	     for(int i=0;i<n;i++){
	     cin>>a[i];
       if(a[i]>10)
	     sum+=(a[i]-10);
       }
	cout<<sum<<endl;  
  sum=0;  
	}
	
	return 0;
}
