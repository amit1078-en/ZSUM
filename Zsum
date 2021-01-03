#include <bits/stdc++.h> 
using namespace std;  
#define endl "\n"
#define ll long long int
#define mod 10000007
ll l=10000;
ll power(ll a,ll k)
{
	ll res=1;
	ll loop=k;
	while(loop>0)
	{
		if(loop%2==0)
		{
			a=((a%mod)*(a%mod))%mod;
			loop/=2;
		}
		else
		{
			res=((res%mod)*(a%mod))%mod;
			loop--;
		}
	}
	res=(res%mod);
	return res;
}
int main()
{
	ll N,K;
	ll first=0;
	ll second=0;
	while(l--)
	{
			cin>>N>>K;
			if(N==0 && K==0)
			{
				break;
			}
			else
			{
				ll p1;
				ll p2;
				second=power(N-1,K);
				first=power(N,K);
				
				p1=power(N-1,N-1);
				p2=power(N,N);
				second=(second+second)%mod;
				p1=(p1+p1)%mod;
				
				cout<<((((p1+p2)%mod+second)%mod+first)%mod)%mod<<endl;
			}	
	}
	return 0;
}
