## EXERCICIOS DE REVISAO
public class Prova01 {

    public static void Soma() {
        Scanner a = new Scanner(System.in);
        System.out.println("quantidade de elementos ");
        int tamanho = a.nextInt();
        int[] vetor = new int[tamanho];
        int soma = 0;
        System.out.println("digite dois valores: ");
        for (int i = 0; i < tamanho; i++) {
            vetor[i] = a.nextInt();
            soma += vetor[i];
        }
        System.out.println("soma dos elementos: " + " terceiro valor= " + soma);
        a.close();
    }

    public static void main(String[] args) {
        Soma();
    }

}
package prova02;

import java.util.Scanner;

public class Prova02 {

    public static void Maior() {
        Scanner a = new Scanner(System.in);
        System.out.println("quantidade de elementos: ");
        int n = a.nextInt();
        int[] vetor = new int[n];
        int n1 = Integer.MIN_VALUE;
        System.out.println("digite os elementos do vetor: ");
        for (int i = 0; i < n; i++) {
            vetor[i] = a.nextInt();
            if (vetor[i] > n1) {
                n1 = vetor[i];
            }
}
            System.out.println("elemento maior: " + n1);
         
   
    }

    public static void main(String[] args) {
        Maior();
    }

}

public static void main(String[] args) {
        Media();
    }

    public static void Media() {
        Scanner l = new Scanner(System.in);
        System.out.println("Digite a quantidade de elementos: ");
        int t = l.nextInt();

        System.out.println("Elementos = ");
        double[] v1 = new double[t];
        
        double soma = 0;
        double media = 0;
        for (int i = 0; i < v1.length; i++) {
            v1[i] = l.nextDouble();
            soma += v1[i];
            media = soma / t;
        }
        System.out.println("A media é = " + media );
    }

}

package provao4;

public class Provao4 {

    public static void Copia() {
        int[] n = new int[]{10, 11, 13, 15};
        int[] n1 = new int[]{16, 17, 18, 19};
        int[] copia = n.clone();
        int[] copia1 = n1.clone();
        for (int i = 0; i < n.length; i++) {
            System.out.println(n[i]);
        }
        for (int i = 0; i < n1.length; i++) {
            System.out.println(n1[i]);
        }

    }

    public static void main(String[] args) {
        Copia();
    }

}
package prova5;

import java.util.Arrays;

public class Prova5 {
    public static void Iguais(){
     int[] n = new int[]{1,2,3};
       int[] n1 = new int[]{1,2,3};
       for (int i = 0; i < n.length; i++) {
           System.out.println(n[i]);
    }for (int i = 0; i < n1.length; i++) {
        System.out.println(n1[i]);
        
    }boolean iguais = Arrays.equals(n, n1);
}
public static void main(String[] args) {
      Iguais();
    }
    
}
package prova6;


public class Prova6 {
    public static void Valor(){
  int[] vetor = { 1, 2, 3, 4, 5 };
int tamanhoVetorOriginal = vetor.length;
int[] vetor_copia = new int[tamanhoVetorOriginal];
int tamanhoVetorOriginalZeroBased = tamanhoVetorOriginal - 1;
for(int i = 0; i < tamanhoVetorOriginal; i++) {
    vetor_copia[i] = vetor[tamanhoVetorOriginalZeroBased - i];
    System.out.print(vetor_copia[i]);
}
    }
public static void main(String[] args) {
     Valor();
    }
    
}
package prova7;

import java.util.Scanner;

public class Prova7 {
    public static void imparesPares(){
     Scanner a = new Scanner(System.in);
        System.out.println("quantidade de elementos: ");
        int n = a.nextInt();
        int[] vetor = new int[n];
        int pares = 0;
        int impares = 0;
        System.out.println("digite os elementos do vetor: ");
        for (int i = 0; i < n; i++) {
            vetor[i] = a.nextInt();
            if(vetor[i] % 2 == 0){
                pares++;
            }else {
                impares++;
            }         
        }
        System.out.println("quantidade de pares: " + pares);
        System.out.println("quantidade de impares" + impares);
        a.close();
    }
public static void main(String[] args) {
     imparesPares();
    }
    
}
package prova8;
import java.util.ArrayList;
import java.util.Scanner;
public class Prova8 {
    public static void Remocao(){
        Scanner a = new Scanner(System.in);
    System.out.println("quantidade de elementos: ");
    int n = a.nextInt();
    int[] vetor = new int [n];
    System.out.println("digite os elemetos do vetor: ");
    for (int i = 0; i < n; i++) {
  
      vetor[i] = a.nextInt();
    }
    System.out.println("digite o valor a ser removido");
    int valorRemovedor = a.nextInt();
    
    ArrayList<Integer> novoVetor = new ArrayList<>();
    for (int i = 0; i < n; i++) {
        if(vetor[i] != valorRemovedor){
            novoVetor.add(vetor[i]);
                }
    System.out.println("vetor resultado apos remocao: ");
    for (int num : novoVetor) {
        System.out.println(num +"");
    }
    a.close();
        }
    }
public static void main(String[] args) {
      Remocao();
    }
    
}
package prova9;
import java.util.Arrays;
import java.util.Scanner;
public class Prova9 {
    public static void Crescente(){
         Scanner a = new Scanner(System.in);
     System.out.println("quantidade de elementos: ");
     int n = a.nextInt();
     int[] vetor = new int[n];
     
     System.out.println("digite os elementos do vetor: ");
     for (int i = 0; i < n; i++) {
        vetor[i] = a.nextInt();
    }
     Arrays.sort(vetor);
     System.out.println("vetor ordenado em ordem crescente; "+ Arrays.toString(vetor));
     a.close();
    }
public static void main(String[] args) {
    Crescente();
    }
    
}


package prova;
import java.util.Scanner;
import java.util.Arrays;

public class Prova {
  public static void Busca() {
        Scanner l = new Scanner(System.in);
        System.out.println("Quantidade de elementos:  ");
        int t = l.nextInt();
        int[] v = new int [t];
        
        System.out.println("Elementos:  ");
        for (int i = 0;i < v.length;i++){
            v[i] = l.nextInt();
        }
        
        System.out.println("Elemento que deseja buscar:   ");
        
        int b = l.nextInt();
        b = Arrays.binarySearch(v,b);
        System.out.println(b);
    }
    public static void main(String[] args) {
        Busca();
    }
    
}