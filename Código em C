#include<stdio.h>
#include<math.h>

//chamada do menu inicial
void menu(){
	printf("-----------------\n");
	printf("[MENU PRINCIPAL]\n");
	printf("\n");
	printf("[ 1 ] - INICIAR\n[ 2 ] - SAIR\n");
	printf("-----------------\n");
}

// funcao que caucula o fatorial de um numero
int fatorial(double n){
	if (n == 1) return 1;
	
	return n * fatorial(n - 1);
}

// funcao que realiza os cauculos
void resultado(double n1, double n2, char es){
	switch (es){
			case '+':
				printf("[%.0lf + %.0lf = %.2lf]\n",n1, n2, n1 + n2);
				break;
			case '-':
				printf("[%.0lf - %.0lf = %.2lf]\n", n1, n2, n1 - n2);
				break;
			case '*':
				printf("[%.0lf × %.0lf = %.2lf]\n", n1, n2, n1 * n2);
				break;
			case '/':
				printf("[%.0lf / %.0lf = %.2lf]\n", n1, n2, n1 /n2);
				break;
			case '!':
				printf("[%.0lf! = %.0lf]\n", n1, fatorial(n1));
				break;
			case 'r':
				printf("[✓%.0lf = %.2lf]\n", n1, (int)sqrt( n1));
				break;
			case '^':
				printf("[%.0lf^%d = %.2lf]\n", n1, n2, (int)pow(n1,n2));
		}
}

// funcao principal
int main (){
	printf("CAUCULADORA SIMPLES\n");
	printf("\n");
	
	while (1){
		int n;
		
		menu();
		
		do{
			printf("Digite sua opcao:");
			scanf("%d", &n);
		}while(n != 1 && n != 2);
		
		//saida do loop caso o usuario escolha 2
		if (n == 2) break;
		getchar();
	
		char es;
		
		// escolha da opcao de cauculo
		printf("\n");
		printf("-----------------\n");
		printf("Escolha umas das opcoes abaixo:\n");
		
		printf("\n");
		
		printf("[ + ] - ADICAO \n[ - ] - SUBTRACAO \n[ * ] - MULTIPLICACAO \n[ / ] - DIVISAO \n[ ! ] - FATORIAL \n[ r ] - RAIZ QUADRADA \n[ ^ ] - POTENCIACAO\n");
		printf("\n");
		printf("-----------------\n");
		// fim
		
		do{
			printf("opcao escolhida:");
			scanf("%c", &es);
			getchar();
		}while(es != '+' && es != '-' && es != '*' && es != '/' && es != 'r' && es != '^' && es != '!');
		
		printf("\n");
		
		// usuario escolhe o(s) numero(s)
		double n1, n2;
		
		if (es == '!' || es == 'r'){
			printf("Digite o numero:");
			scanf("%lf", &n1);
		}
		else{
			printf("Digite os 2 numeros:");
			scanf("%lf %lfp", &n1, &n2);
		}
		
		//saida do resultado
		printf("Resultado.....\n");
		printf("\n");
		
		resultado(n1, n2, es);
		printf("\n");
	}
	
	
	// fim da secao
	printf("\n");
	printf("SECAO FINALIZADA - VOLTE SEMPRE!\n");
	
	return 0;
	
}
