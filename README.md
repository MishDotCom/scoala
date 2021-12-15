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
### → Eliminarea Unei Cifre
```cpp
int n,m,p;
cin>>n;
//p se initializeaza cu elementul neutru al inmultirii
p=1;
//construim numarul m cu cifrele impare ale lui n, astfel m o sa reprezinte numarul format prin eliminarea cifrelor pare
while(n>0)
{
    if(n%2==1)//se verifica daca cifra este impara
    {
         m=(n%10)*p+m;// se adauga cifra pe pozitia corespunzatoare in numarul nou format(unitati, zeci, sute etc.)
         p=p*10;//se mareste puterea lui 10, pentru ca urmatoarea cifra impara sa fie adaugata din nou pe pozitia corespunzatoare(zeci, sute, mii etc.)
    }
    n=n/10;
{
```
