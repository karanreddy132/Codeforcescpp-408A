# Codeforcescpp-408A
#include <bits/stdc++.h>
using namespace std;

int main() {
	int n,k[101],m;
  vector<int> v;
  cin >> n;
  for(int i=0;i<n;i++)
    cin >> k[i];
  
  for(int i=0;i<n;i++){
    int sum = 0;
    for(int j=0;j<k[i];j++){
      cin >> m;
      sum+=m*5 + 15;
    }
    v.push_back(sum);
  }
  cout << *min_mment(v.begin(),v.end());
  return 0;
}
