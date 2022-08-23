
package javaapplication5;

import java.util.Scanner;
public class JavaApplication5 {

   
    public static void main(String[] args) {
        Scanner leer = new Scanner(System.in);
        int n, tipoVend;
        String cedula;
        double valorVent,comision1,comision2;
        
        System.out.println("digite numero de vendedores: ");
        n = leer.nextInt();
        
        
        for (int i=0;i<n;i++){
            System.out.println("digite cedula: ");
            cedula = leer.next();

            System.out.println("digite tipo de vendedor: ");
            tipoVend = leer.nextInt();

            System.out.println("digite valor en ventas: ");
            valorVent = leer.nextDouble();
            if (tipoVend==1){
                comision1 = valorVent * 0.20;
                System.out.println("la comision del vendedor puerta a puerta es: "+comision1);
            }
            else{
                comision2 = valorVent * 0.30;
                System.out.println("la comision del vendedor ejecutivo es: "+comision2);
            }
        
        }
        
    }
    
}
