  #include <stdio.h>
	#include <stdlib.h>

	//Funções
	void soma(float a, float b){
		printf("Resultado: %.2f\n", a + b);
	}
	void sub(float a, float b){
		printf("Resultado: %.2f\n", a - b);
	}
	void mult(float a, float b){
		printf("Resultado: %.2f\n", a * b);
	}
	void divi(float a, float b){
		if(b != 0){
		printf("Resultado: %.2f\n", a / b);	
		} else {
			printf("Operacao Inválida!");
		}
	}
	
	int main()
	{
		int opcao = -1;
		float num1; float num2;
		
		while(opcao != 0) {
		
		
		printf("\n===== CALCULADORA =====\n");
		printf("1 - Soma\n");
		printf("2 - Subtracao\n");
		printf("3 - Multiplicacao\n");
		printf("4 - Divisao\n");
		printf("0 - Sair\n");
		printf("\nEscolha uma opcao: ");
		scanf("%d", &opcao);
		
		if(opcao >= 1 && opcao <= 4){

		printf("\nDigite o primeiro operador: ");
		scanf("%f", &num1);
		
		printf("\nDigite o segundo operador: ");
		scanf("%f", &num2);
	}
		switch(opcao){
			case 1:
				soma(num1, num2);
				break;
			case 2:
				sub(num1, num2);
				break;
			case 3:
				mult(num1, num2);
				break;
			case 4:
				divi(num1, num2);
				break;
			case 0:
				printf("\nSaindo...");
				break;
			default:
				printf("\nOpcao Invalida!!");
				
		}
	}
		
		
		return 0;
	}
