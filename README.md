# actividad2_punto3_poo
package triangulo;
import java.util.Scanner;
public class Triangulo {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        double  lado1,lado2,lado3,perimetro,semipe,area;
        Scanner ingresotec = new Scanner (System.in);
        
        System.out.println("Ingrese el lado 1 del triangulo:  ");
        lado1 = ingresotec.nextDouble();
        
        System.out.println("Ingrese el lado 2 del triangulo:  ");
        lado2 = ingresotec.nextDouble();
        
        System.out.println("Ingrese el lado 3 del triangulo:  ");
        lado3 = ingresotec.nextDouble();
        
        perimetro= lado1 + lado2 + lado3;
        semipe= perimetro/2;
        area= Math.sqrt((semipe)*(semipe-lado1)*(semipe-lado2)*(semipe-lado3));
        
        System.out.println("el perimetro es :  "+ perimetro);
        System.out.println("el semiperimetro es :  "+ semipe);
        System.out.println("el area es: "+ area);
        
    }
    
}
