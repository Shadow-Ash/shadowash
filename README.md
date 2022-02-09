#include<iostream.h>
#include<conio.h>
class ratio
{
int num,den;
public:
	void assign(int n,int d)
	{
		num=n;
		den=d;
	}
	void convert();
	void invert();
	void print();
};
void ratio::convert()
{
	cout<<"the ratio is "<<double(num)/double(den);
}
void ratio::invert()
{
	int temp;
	temp=num;
	num=den;
	den=temp;
}
void ratio::print()
{
	cout<<"\n the values are "<<num<<"/"<<den<<"\n";
}
void main()
{
	clrscr();
	ratio r;
	r.assign(22,7);
	r.convert();
	r.print();
	r.invert();
	cout<<"After inverting the values ";
	r.print();
	getch();
}
