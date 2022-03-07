# Capgemini

Dasafio 1 - Resposta:

E-mail classificado como #EXTERNO.CONFIDENCIAL

import java.util.Arrays;

public class Main {
    public static void main(String[] args) {

        // Conjunto informado no exercício
        int arr[] = { 9, 2, 1, 4, 6 };

       
        Arrays.sort(arr);

        int mediana;
        int metade = arr.length / 2;
        
        // Caso o conjunto fosse par, a função faz a média dos valores centrais
        if (arr.length % 2 == 0) {
            mediana = (arr[metade - 1] + arr[metade]) / 2;
        } else {
            mediana = arr[metade];
        }

        // Imprimir valores
        System.out.println("O conjunto “arr” ordenado é apresentado abaixo: ");
        for (int x = 0; x < arr.length; x++) {
            System.out.printf("%d ", arr[x]);
        }
        System.out.printf("\nA mediana do conjunto “arr” é:%d", mediana);

    }
