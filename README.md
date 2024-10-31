- 👋 Hi, I’m @tiamat-droid
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

#include <stdio.h>
// 1. Criar o menu principal
//Você deve fazer um menu pedindo para o usuário escolher entre as seguintes
//opções: Use a variável continuaMenu para repetição
//●  Cadastrar novas vendas
//● Ver informações de uma venda específica, baseado no nome do cliente
//● Ver informações de todas as vendas
//● Encerrar o programa


//função 1: menu de opção
// vai imprimir o menu de opções sem retorno:
//! 1- Cadastrar novas vendas
//! 2- Ver informações de uma venda específica, baseado no nome do cliente
//! 3- Ver informações de todas as vendas
//! 4-  Encerrar o programa

//função 2:  com retorno
//vai fazer a leitura da opção q o usuário vai digitar

//? -----------primeira função--------------

void menu(){
    printf("SELECIONE UMA OPÇÃO:\t ");
    printf("\t1-Cadastrar novas vendas\n");
    printf("\t2-Ver informações de uma venda específica, baseado no nome do cliente\n");
    printf("\t3- Ver informações de todas as vendas\n");
    printf("\t4-Encerrar o programa\n");
}
    //?-----------segunda função-------------- 

    int ler_opcao() {
        int op;
    
        while(1){
        printf("digite a sua opção: ");
        scanf("%d", &op);
        
        switch (op){
            case 1:
             printf("1-Cadastrar novas vendas");
             break;
            case 2:
             printf ("2-Ver informações de uma venda específica, baseado no nome do cliente");
             break;
            case 3:
            printf("3- Ver informações de todas as vendas");
            break;
            case 4:
             printf("4-Encerrar o programa");
              //vl=1;
              return op;

         default:
             printf("opção inválida");
             menu();
        } 
    }
}

int main(){
    
    int opc;
    menu();
    opc = ler_opcao();

    //fazer as coisas
   printf ("a opção é %d:", opc);

return 0;
}
