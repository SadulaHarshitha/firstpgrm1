# firstpgrm1
singulartoplural
#include <iostream>
#include <string>
using namespace std;

int main ()
{
	string 	str,str2;
	int	n;
	char	ch,ch2;

		cin>>str;
		n=str.length();
		ch=str[n-1];
		ch2=str[n-2];

		if (ch=='y')
		{	
			if(ch2=='a' || ch2=='e' || ch2=='i' || ch2=='o' || ch2=='u')
			str2=str+"s";
			else
			str2=str.substr(0,n-1)+"ies";
		}
		else if(ch=='s' && ch2=='i')
			str2=str.substr(0,n-2)+"es";
		else if (ch=='o'||ch=='s'||ch=='x')
			str2=str+"es";
		else if (ch=='h'&& ch2=='c')
			str2=str+"es";
		else if (ch== 'f')
			str2=str.substr(0,n-1)+"ves";
		else if (ch=='e'&&ch2=='f')
			str2=str.substr(0,n-2)+"ves";
		else
			str2=str+"s";
		
		cout<<str<<"plural is: "<<str2<<endl;
}
