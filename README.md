# the-work-of-hanwh
#include<iostream>
#include<string>
#include<cmath>
using namespace std;
int main() {
	string a; int b = 0; int c = 0; char d = '.'; double e = 0; int g = 0;
	cin >> a;
	b = size(a);
	for (int i = 0; i < b; i++)
	{
		if (a[i] == d)
		{
			c = i;
         }
	}
	if (c == 0)
	{
		for (int i = 0; i < b; i++)
		{
			int  f = pow(8, b - 1 - i) * ((int)a[i]-48);
			g = g + f;
		}
		cout << g << endl;
	}
	else
		for (int i = 0; i < b; i++)
		{
			if (i != c )
			{
				double f = pow(8, c - i ) * ((int)a[i]-48);
				e = e + f;
			}
			cout << e << endl;
		}
	
}
