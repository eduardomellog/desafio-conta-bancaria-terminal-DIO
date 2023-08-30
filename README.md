# Desafio de conta bancária no terminal, inicio do bootcamp Santander Backend Java.


Código simples e intuitivo, mensagens no terminal direcionam o usuário e utilizei o Scanner como proposto no exercício.

Ao final é exibida uma mensagem de conta criada.

Fique a vontade para acessar o caminho conta-bancaria/src/ContaTerminal.java

Segue o código:

```

import java.util.Scanner;

public class ContaTerminal {
    public static void main(String[] args) throws Exception {
        
        Scanner entrada = new Scanner(System.in);

        int numero = 0;
        String agencia = "";
        String nomeCliente = "";
        float saldo = 0.0F;

        System.out.println("Olá cliente, vamos criar uma conta em nossa agência?");

        System.out.println("Por favor, digite um número de conta com 4 dígitos, sendo eles entre 0 e 9: ");
        numero = entrada.nextInt();

        System.out.println("Por favor, digite o número da agência, respeitando o formato de 3 digitos, um traço e um dígito final. Exemplo: 000-0: ");
        agencia = entrada.next();

        System.out.println("Por favor, digite o nome completo do cliente: ");
        
        entrada.nextLine();
        
        nomeCliente = entrada.nextLine();

        System.out.println("Agora digite o saldo inicial da sua conta corrente: ");
        saldo = entrada.nextFloat();
    
        entrada.close();
    
        System.out.println("Olá " + nomeCliente + ", obrigado por criar uma conta em nosso banco, sua agência é: " + agencia + ", conta: " + numero + " e seu saldo: " + saldo + " já está disponível para saque!");
    }
}

```
