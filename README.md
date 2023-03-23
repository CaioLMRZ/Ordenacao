import java.security.SecureRandomParameters;
import java.util.Arrays;
import java.util.Scanner;
import java.util.Random;

public class TrabalhoOrdencaoRogerio2 {
	


static Random random = new Random();
 
	public static void main(String[] args) {
		
		
int numeros [] = {0, 0, 0, 0, 0, 0, 0, 0, 0, 0};
       //Posições{0, 1, 2, 3, 4, 5, 6, 7, 8, 9}

		
System.out.println("Digite 10 numeros:"+" ");
for (short i = 0; i < numeros.length; i++) {
    numeros[i] = random.nextInt(5000) ;
}

  
  System.out.print("Números Escolhidos: ");
  
            for(int valor:numeros) {
			System.out.print(valor+" ");
		}
     
            Arrays.sort(numeros);

            System.out.println();
            
            System.out.print("Os numeros em ordem crescente:");
            
            for(int valor:numeros) {
    			System.out.print(valor+" ");
    		}
            
            System.out.println("");
            
            
            System.out.print("Os numeros em ordem decrescente:");
            for (short i = (short)(numeros.length - 1); i >= 0; i--) {
                System.out.print(numeros[i] + " ");
            }
         
	}

}
