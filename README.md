# ✅ Materie Pentru Teza La Info

## ↺ Algoritmi

### → Divizorii Unui Numar
```cpp
int n;
cin >> n;
for (int d = 1; d * d <= n; d++){}
    if (n % d == 0){
        cout << d;
        int k = n / d;
        if (k != d)
            cout << k;
    }
}
```
### → CMMDC
```cpp
int n, m;
cin >> n >> m;
while (m != 0) {
    int r = n % m;
    n = m;
    m = r;
}
cout << n;
```
### → CMMMC
```cpp
int n, m, a, b;
cin >> a >> b;
n = a;
m = b;
while (m != n) {
    if (n < m)
        n += a;
    else if (n > m)
        m += b;
}
cout << m;
```
### → Numere Prime
```cpp
//generalizat
bool isPrime(int n) {
	if (n < 2)
		return false;
	for (int d = 2; d * d <= d; d++) {
		if (n % d == 0)
			return false;
	}
	return true;
}
```
### → Oglinditul Unui Numar
```cpp
int n, ogl = 0;
cin >> n;
while (n != 0)
{
    ogl = ogl * 10 + n % 10;
    n = n / 10;
}
cout <<  ogl;
```
### → Descompunerea In Cifre
```cpp
// n = numar; c = cifra;
int n,c;
cin >> n;
while (n != 0){
    c = n % 10;
    n = n / 10;
    cout << c << " ";
}
```
