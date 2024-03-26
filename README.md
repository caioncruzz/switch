//programa que recebe um caractere para informar a raça do usuário

# include <stdio.h>
# include <stdlib.h>
# include <locale.h>

int main ()

{
	setlocale (LC_ALL, "Portuguese");
	
	char raca;
	
	printf ("Informe sua raça\n");
	printf ("A: Preto(a)\n");
	printf ("B: Branco(a)\n");
	printf ("C: Pardo(a)\n");
	printf ("D: Indígena\n\n");
	
	scanf ("%c,", &raca);
	
	switch (raca) {
	case 'A': case 'a':
		printf ("\nPreto(a)\n\n");
		break;
	case 'B': case 'b':
		printf ("Branco(a)\n\n");
		break;
	case 'C': case 'c':
		printf ("Pardo(a)\n\n");
		break;
	case 'D': case 'd':
		printf ("Indígena\n\n");
		break;
	default:
		printf ("Não informado\n\n");
	}

system ("pause");
return 0;

}
