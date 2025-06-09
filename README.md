//# TP4-1R7-UTN-FRC
#include <stdio.h>

int main ()
	
{
	char repetir;
   do{
		float peso=0.0,altura=0.0,imc=0.0;
		
		
		
		printf("este programa calcula el indice de masa corporal\n");
		printf("debe ingresar el peso en kg de la persona\n");
		scanf("%f",&peso);
		printf("ingrese la altura en metros de la persona\n");
		scanf("%f",&altura);
		imc=peso/(altura*altura);
		printf("el indice de masa corporal es:%f\n",imc);
		printf("\n");
		printf("\n");
		
		printf("indice|condicion\n");
		
		printf("...............................\n");
		printf("<18.5|bajo peso\n");
		printf("18.5 a 24,9|normal\n");
		printf("25.0 a 29.9|sobrepeso\n");
		printf(">=30|obesidad\n");
		
		
		
		if (imc<=18.5)
		{ printf("su imc es: %2.f lo cual es bajo\n",imc);
		}else if (imc>=18.5&&imc<=24.9)
		{printf("su imc es: %2.f lo cual esta dentro de los parametros normales\n",imc);
		}else {
				  printf("su imc es: %2.f lo que indica obesidad\n",imc); 
				  
		} printf("desea repetir el programa? s/n\n");
		scanf(" %c",&repetir);
		
   }while (repetir=='s'||repetir=='S');
		
		
		
		
		
		return 0;
	}
	

	
