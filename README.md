# gerador-de-senha
gerador simples de senhas aleatórias, ele utiliza 70 caractéres diferentes do teclado e os sorteia para o tamanho que o usuario insere. 

# como funciona 
O usuário insere o tamanho da senha desejado (ex: 8 caractéres) e o computador retorna para o usuário uma senha aleatória com letras(maiuscúlas e minúsculas), números e simbolos com a quantidade de caractéres desejados pelo usuário(tamanho da senha). 

# Recursos
- Java
- Scanner
- Random
- loop
- length

# Código inteiro:
    package geradordesenhas;
    import java.util.Scanner;
    import java.util.Random;

    public class Geradordesenhas {

    
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);
        Random rnd = new Random();
        
        System.out.println("Digite o tamanho da senha: ");
        int tamanho = leitor.nextInt();
        
        String caracteres = "QWERTYUIOPASDFGHJKLÇZXCVBNMqwertyuiopasdfghjklçzxcvbnm0123456789!@#$%&";
        rnd.nextInt(caracteres.length());
        String senha = "";
        for(int i = 0; i < tamanho; i++){
            int indice = rnd.nextInt(caracteres.length());
            char caractere = caracteres.charAt(indice);
            senha += caractere;
            
            
        }
    System.out.println("Senha gerada: " + senha);    
        
                
        
        
    }
    
    }


# Código sem a estrutura básica:

    Scanner leitor = new Scanner(System.in);
        Random rnd = new Random();
        
        System.out.print("Digite o tamanho da senha: ");
        int tamanho = leitor.nextInt();
        
        String caracteres = "QWERTYUIOPASDFGHJKLÇZXCVBNMqwertyuiopasdfghjklçzxcvbnm0123456789!@#$%&";
        rnd.nextInt(caracteres.length());
        String senha = "";
        for(int i = 0; i < tamanho; i++){
            int indice = rnd.nextInt(caracteres.length());
            char caractere = caracteres.charAt(indice);
            senha += caractere;
            
            
        }
    System.out.println("Senha gerada: " + senha);    
        
  

