#include <stdio.h>
#include <stdlib.h>
#include <time.h>

void main(int argc, char *argv[])
{
    int min, max, resultado;

    if (argc < 3)
    {
        printf("Você precisa informar os limites para geração do número\n");
        printf("Made By Davi Sales");
        exit(0);
    }

    min = atoi(argv[1]);
    max = atoi(argv[2]);

    srand(time(NULL));

    resultado = min + rand() % (max - min + 1);

    printf("O número aleatório é %d\n", resultado);

    printf("Made by Davi Sales");
}
