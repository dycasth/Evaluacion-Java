import java.util.Scanner;

public class Rectangulo {

	Scanner teclado = new Scanner(System.in);

	int n; int b; int bx;

	public void entradato(){


		System.out.println("ingrese un numero entre 1 y 9 ");
		System.out.print("ingrese largo:   ");
		n = teclado.nextInt();

		System.out.print("ingrese ancho:   ");
		b = teclado.nextInt();

		if(n == 0  && n <= 9 ){
			System.out.println(" Numero no valido ingrese un numero entre 1 y 9 ");


		}

	}

	public void proceso(){

        
		if(n >= 1  && n <= 9 )
			for (int i = 1; i<= n; i++){
				for (int j = 1; j<=b; j++){
					if (i==1 || i==n || j==1 || j==b){
				       System.out.print(b);
					}
					else if (i==2 || i==n-1 || j==2 || j==b-1){
				        System.out.print(b-1);
				    }
					else{
						System.out.print(b-2);

					}

			     }
			     System.out.println("");
			 }
		}
	

    public static void main(String args[]){

   Rectangulo fc = new Rectangulo();
   fc.entradato();
   fc.proceso();
   }
}