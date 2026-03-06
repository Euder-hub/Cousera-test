#include <stdio.h>
#include <stdlib.h>
#include <iostream>
#include <conio.h>

using namespace std;

struct status{
	unsigned int ligado:1;
	signed int valor:4;
	unsigned int num:3;
};

void check_status(struct status s)
{
	if (s.ligado == 1)
		printf("LIGADO\n");
		printf("\n\n%f\n",&s);
	if (s.ligado == 0)		
		printf("DESLIGADO\n");
		printf("\n\n%f\n",&s);
	return ;
	
}

int main()
{
	char quit;
    quit = '\0';
    float n=0;

	ini:
		//system("cls");
	puts("\nStatus:\n");	
     scanf("\n%f",&n);  
	
	struct status ESTADO;
		   ESTADO.ligado= n;
		   check_status(ESTADO);
		   system("pause");
		
	//return 0;
	getch();
	goto ini;
		
}
