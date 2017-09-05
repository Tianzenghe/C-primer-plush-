#include<iostream>
using namespace std;
int main()
{
	const char* brid = "wren";
	cout << brid << endl;
	char * pbrid = "pwren";
	cout << *pbrid << pbrid << endl;//一般来说,如果给cout提供一个指针,它将打印地址.
									//但如果指针的类型为 char* ,则cout将显示指向字符串.
	cout << (int *)pbrid << endl;
	//如果要显示的是字符串的地址,则必须将这种指针强制转换为另一种指针类型.

	int aa[3] = { 1,2,3 };
	int *p = aa;
	cout << p << endl << *p;
	return 0;
}
