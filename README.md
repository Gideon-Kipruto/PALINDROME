# PALINDROME
# include <iostream>
using namespace std;
char pall (string w);
int main()
{
	string m;
	cout << "enter a name:";
	cin >> m;
	cout << (pall (m) ? "true" :  "false");
}
char pall (string w)
{
	int pos = 0;
	int neg = w.length() - 1;
	while (pos < neg)
	{
		if(w[pos] != w[neg])
		{
			return false;
		}
		pos++;
		neg--;
	}
	return true;
}
