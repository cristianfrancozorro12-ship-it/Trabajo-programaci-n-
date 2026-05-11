// Clase principal, donde inicia la ejecución
public class Pago {
    public static void main(String[] args) {

        /* Se crea el objeto trabajador1, de la clase Empleados por
        comisión (Emp_comision) */
        Emp_comision trabajador1 = new Emp_comision(5, "Policarpo Alva", 'C');

        // El trabajador 1 realiza 2 ventas
        trabajador1.vender(2000.89f);
        trabajador1.vender(1000);

        // se muestra la información del trabajador1
        trabajador1.mostrar_info();

        // Calcula e imprime el pago del trabajador1
        System.out.printf("Su pago es de $%.2f \n", trabajador1.calc_pago());

        /* Se crea el objeto trabajador2, de la clase Empleados por horas
        (Emp_horas) */
        Emp_horas trabajador2 = new Emp_horas(8, "Simplicio Bejarano", 'B', 250, 'N');

        // El trabajador2 acumula horas trabajadas en 3 ocasiones
        trabajador2.acum_horas(5);
        trabajador2.acum_horas(10);
        trabajador2.acum_horas(3);

        // se muestra la información del trabajador 2
        trabajador2.mostrar_info();

        /* Calcula e imprime el pago del trabajador2, con la primera ver-
        sión de calc_pago() */
        System.out.printf("Su pago es de $%.2f \n", trabajador2.calc_pago());

        /* Calcula e imprime el pago del trabajador2, con la segunda ver-
        sión de calc_pago() */
        System.out.printf("Su pago sería de $%.2f \n", trabajador2.calc_pago('A'));

        /* Se crea el objeto trabajador3, de la clase Empleados por comisión
        (Emp_comision) */
        Emp_comision trabajador3 = new Emp_comision(3, "Hortencia Ruiz", 'C');
        
    }
}
