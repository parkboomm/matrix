int main()
{
    float matrix[4][4];
    int i, j,cont;
    float somarpar, somarimpar;
    float media;
    somarimpar = 0;
    somarpar = 0;
    cont = 0;
    
    for(i = 0; i < 4; i++){
        for(j = 0; j < 4; j++){
        printf("digite um número inteiro:" );
        scanf("%f", &matrix[i][j]);
    }
    
   }
   for(i = 0; i < 4; i++){
        for(j = 0; j < 4; j++){
            if(j % 2 == 0){
                somarpar = somarpar + matrix[i][j];
                cont = cont + 1;
            }
            else {
                somarimpar = somarimpar + matrix[i][j];
            }
        }
   }
media = somarimpar/cont;

printf("A soma dos valores das colunas impares é %f",somarimpar);
printf("A soma dos valores das colunas pares é %f",somarpar);

    return 0;
}
