import java.util.Scanner;
public class Simulacro {
    public static void main(String[] args) {
        Scanner tcl = new Scanner(System.in);
        String tipoEvento, cantDescuento;
        int numEntradas =0, tipoUsuario =0, tarjetaFestival =0, cont =1;
        double descuento, preciounitario =0, costo, totalPagar;
        while (cont <= 3) {
            System.out.print("INGRESA A QUE EVENTO DESEAS INGRESAR: ");
            tipoEvento = tcl.next();
            switch (tipoEvento){
                case "Teatro":
                    preciounitario = 15;
                    System.out.print("INGRESA EL NUMERO DE ENTRADAS QUE DESEA COMPRAR: ");
                    numEntradas = tcl.nextInt();
                    System.out.print("TIPO DE USURARIO COLACA 1 SI ES ESTUDIANTE, 2 SI ES ADULTO MAYOR: ");
                    tipoUsuario = tcl.nextInt();
                    System.out.print("POSEE TARJETA DE DESCUENTO? COLA UN 1 (SI) O 2 (NO): ");
                    tarjetaFestival = tcl.nextInt();
                    break;
                case "Musica":
                    preciounitario = 10;
                    System.out.print("INGRESA EL NUMERO DE ENTRADAS QUE DESEA COMPRAR: ");
                    numEntradas = tcl.nextInt();
                    System.out.print("TIPO DE USURARIO COLACA 1 SI ES ESTUDIANTE, 2 SI ES ADULTO MAYOR: ");
                    tipoUsuario = tcl.nextInt();
                    System.out.print("POSEE TARJETA DE DESCUENTO? COLA UN 1 (SI) O 2 (NO): ");
                    tarjetaFestival = tcl.nextInt();
                    break;
                case "Artes":
                    preciounitario = 8;
                    System.out.print("INGRESA EL NUMERO DE ENTRADAS QUE DESEA COMPRAR: ");
                    numEntradas = tcl.nextInt();
                    System.out.print("TIPO DE USURARIO COLACA 1 SI ES ESTUDIANTE, 2 SI ES ADULTO MAYOR: ");
                    tipoUsuario = tcl.nextInt();
                    System.out.print("POSEE TARJETA DE DESCUENTO? COLA UN 1 (SI) O 2 (NO): ");
                    tarjetaFestival = tcl.nextInt();
            }
            cont = cont + 1;
            costo = numEntradas * preciounitario;
            if (tipoUsuario == 1){
                descuento = preciounitario * 0.2;
                System.out.println(cantDescuento += "20%");
            }else{
                descuento = preciounitario * 0.3;
                System.out.println(cantDescuento += "30%");
            }
            if (tarjetaFestival == 1){
                descuento = (preciounitario * 0.1) - descuento;
                System.out.println(cantDescuento += "30%");
            }
        }
        System.out.println(con + ", " + tipoEvento + ", " + preciounitario + ", " + tarjetaFestival + ", " + descuento + ", " + numEntradas + ", " + );
    }
}
