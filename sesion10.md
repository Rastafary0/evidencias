<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


## Actividad 10 

Polimorfismo en Java - Ejercicios prácticos
Practicar el uso de la sobreescritura de métodos para implementar polimorfismo en Java. Resolver los siguientes ejercicios.

Ejercicio 1:
Crea una clase abstracta Vehículo con métodos abstractos acelerar(), frenar() y girar(). Las clases Coche, Moto y Bicicleta heredan de la clase Vehículo y sobreescriben los métodos abstractos para implementar su propio comportamiento.


## Clase Vehiculo

```java

public abstract class Vehiculo {
    
    public abstract void acelerar();
    public abstract void frenar();
    public abstract void girar();

   
    }
```

## Coche

```java
public class Coche extends Vehiculo {

    public Coche() {
    }

    @Override
    public void acelerar() {
       
    }

    @Override
    public void frenar() {
       
    }

    @Override
    public void girar() {
        
    }
    
    
}

```
## Moto

```java

public class Moto extends Vehiculo {

    public Moto() {
    }

    @Override
    public void acelerar() {
        
    }

    @Override
    public void frenar() {
        
    }

    @Override
    public void girar() {
        
    }
    
    
}

```

## Bicicleta

```java

class Bicicleta extends Vehiculo {

    @Override
    void acelerar() {
        System.out.println("La bicicleta acelera");
    }

    @Override
    void frenar() {
        System.out.println("La bicicleta frena");
    }

    @Override
    void girar() {
        System.out.println("La bicicleta gira");
    }
    
}


```
 ## Main 

```java
public static void main(String[] args) {
     ArrayList<Vehiculo> vehiculos = new ArrayList<>();
        vehiculos.add(new Coche());
        vehiculos.add(new Bicicleta());
        vehiculos.add(new Moto());

        for (Vehiculo vehiculo : vehiculos) {    
            vehiculo.acelerar();
            vehiculo.frenar();
            vehiculo.girar();
 ```           
        }
    }



Ejercicio 2:
Crea una clase abstracta Producto con métodos abstractos calcularPrecio() y calcularImpuesto(). Las clases Libro, CD y DVD heredan de la clase Producto y sobreescriben los métodos abstractos para implementar su propio cálculo de precio e impuesto.

Ejercicio 3:
Crea una clase abstracta Cuenta con métodos abstractos depositar(), retirar() y consultarSaldo(). Las clases CuentaCorriente, CuentaAhorro y CuentaPlazoFijo heredan de la clase Cuenta y sobreescriben los métodos abstractos para implementar su propio comportamiento.

Previous



<!-- Su documentación aquí -->





