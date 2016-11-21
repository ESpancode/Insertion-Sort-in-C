//Insertion-Sort-in-C
//Insertion Sort that was created in C

#include <stdio.h> //Standard In/Out
#include <stbool.h> //Standard Boolean
#define NUMAX 8 //Define max number

int array[NUMAX] = {1,2,3,4,5,6,7,8} // Assigning numbers in array

// Counting numbers within the array

void printline(int count) {
int a;
for (a = 0;a < count -1; a++){
    printf("=");

}
printf("=\n");
}

// Display numbers 

void Show(){
    int a;
    printf("{");
    for(a = 0;a<NUMAX; a++){
        printf("%d", NUMAX [a]);
    }
    printf("}\n");
}

// Creating the Insertion Sort

void Insertion() {

   int Insert;
   int Posit;
   int a;
  
   //Creating a loop
   for(i = 1; i < NUMAX; a++) { 
	
      // selecting values
      Insert = NUMAX[a];
		
      // Finding a position for insert
      Posit = a;
		
      // Checking value that is inserted
      while (Posit > 0 && NUMAX[Posit-1] > Insert) {
         NUMAX[Posit] = NUMAX[Posit-1];
         Posit--;
         printf(" Moving Numbers : %d\n" , NUMAX[Posit]);
      }

      if(Posit != a) {
         printf(" NUM Inserted : %d, at position : %d\n" , Insert,Posit);
         // Inserting a number 
         NUMAX[Posit] = Insert;
      }

      printf("Insterted %d#:",a);
      Show();
		
   }  
}

// Printing the value

Main() {
   printf("Import Number: ");
   Show();
   printline(20);
   Insertion();
   printf("Export Number: ");
   display();
   printline(20);
}
