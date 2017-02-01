# Lab1-StarRecur 

#include<iostream> 
using namespace std; 


int star(static int rows)
{
	

     int static rowCount = rows;
     int static starCount = 0;
	
	 if (rowCount==0)
	 {
		 return 0;
	 }

	
	 cout<<"*"; 
	 starCount++; 
	 if (starCount==rowCount)
	 {
		 starCount=0;
		 cout<<endl; 
		 rowCount--; 
		 star(rowCount);
	 }

	 star(rows-1);
	 
        
	

}


int main()
{



	star(12);

	system("Pause"); 
	return 0; 
}
