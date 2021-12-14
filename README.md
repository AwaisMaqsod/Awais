# Awais
Repository for c++ Oop codes. 
//Write a program to overload binary addition operator
#include<iostream>
#include<string>
using namespace std;

class Addition{
	private:
		int a,b;
	public:
		Addition(){
		a=b=0;
		}
		void input(){
			cout<<"Enter first value : "<<endl;
			cin>>a;
			cout<<"Enter first value : "<<endl;
			cin>>b;
			
		}
		Addition operator+(Addition aa){
		Addition temp;
		temp.a=a+aa.a;//1=1+1 ->2
		temp.b=b+aa.b;//2=2+2 ->4
		return temp;
		}
		
		
		
		void show(){
			cout<<"1st value is : "<<a<<endl;
			cout<<"2nd value is : "<<b<<endl;
			
		}
		
		
};

int main(){
	Addition a1,a2,a3;
	a1.input();
	a2.input();
	
	a1.show();
	a2.show();
	
	a3=a1+a2;
	a3.show();
	
	
	return 0;
}
