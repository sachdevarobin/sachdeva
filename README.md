
# sachdeva
Language c++:

Question 1.
Sol:
```
    vector<int> sum(vector<int>& num, int target) {
        unordered_map<int, int> m;
        for (int i = 0; i < num.size(); i++) {
            if (m.find(target - num[i]) != m.end()) {
                return {m[target - num[i]], i};
            }
            m[num[i]] = i;
        }
        return {};
    }
                                   
  ```
  
  Question 2.
  Sol:
  
  ```
  bool palindrome(int n) {
  int t, r = 0;
  t = n;

  while (t != 0) {
    r = r * 10;
    r = r + t%10;
    t = t/10;
  }

  if (n == r)
    return true;
  else
    return false;
}

```
