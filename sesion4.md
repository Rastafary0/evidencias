<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->

## Actividad: Creación de una clase de producto con modificadores de acceso y getters y setters


Objetivo:

Evaluar la capacidad de para crear clases con modificadores de acceso, private, default, protected, final, static. Además, evaluar el uso de getter y setter.

Descripción:

Crear una clase llamada Producto con los siguientes atributos:

nombre: un atributo de tipo String que representa el nombre del producto.
precio: un atributo de tipo double que representa el precio del producto.
cantidad: un atributo de tipo int que representa la cantidad disponible del producto.
fabricante: un atributo de tipo String que representa el fabricante del producto.
marca: un atributo de tipo String que representa la marca del producto.
categoría: un atributo de tipo String que representa la categoría del producto.
Utilizar los modificadores de acceso para controlar el acceso a los atributos de la clase. Por ejemplo, el atributo nombre debería ser público, el atributo precio debería ser privado, el atributo cantidad debería ser protegido, el atributo fabricante debería ser final, el atributo marca debería ser static, y el atributo categoría debería ser default.

Utilizar getter y setter para acceder y modificar los valores de los atributos de la clase. Por ejemplo, el método getNombre() debería devolver el valor del atributo nombre, y el método setNombre() debería establecer el valor del atributo nombre.

Instrucciones:

Cree una clase llamada Producto.
Agregue los atributos nombre, precio, cantidad, fabricante, marca y categoría a la clase Producto.
Utilice los modificadores de acceso para controlar el acceso a los atributos de la clase.
Agregue getter y setter para acceder y modificar los valores de los atributos de la clase.
Pruebe la clase Producto creando una instancia de la clase y accediendo a los atributos de la instancia.

Clase

import java.util.logging.Logger;

/**
 *
 * @author alexander
 */
public class Productos {
    
  public String Nombre;
  private double Precio;
  protected int Cantidad;
  final String Fabricante;
  static String Marca;
  String Categoria;

    public Productos(String Nombre, double Precio, int Cantidad, String Fabricante, String Categoria) {
        this.Nombre = Nombre;
        this.Precio = Precio;
        this.Cantidad = Cantidad;
        this.Fabricante = Fabricante;
        this.Categoria = Categoria;
    }

    public String getNombre() {
        return Nombre;
    }

    public double getPrecio() {
        return Precio;
    }

    public int getCantidad() {
        return Cantidad;
    }

    public String getFabricante() {
        return Fabricante;
    }

    public static String getMarca() {
        return Marca;
    }

    public String getCategoria() {
        return Categoria;
    }

    public void setNombre(String Nombre) {
        this.Nombre = Nombre;
    }

    public void setPrecio(double Precio) {
        this.Precio = Precio;
    }

    public void setCantidad(int Cantidad) {
        this.Cantidad = Cantidad;
    }

    public static void setMarca(String Marca) {
        Productos.Marca = Marca;
    }

    public void setCategoria(String Categoria) {
        this.Categoria = Categoria;
    }
 
       
}




MAIN
public class Actividadad4 {

    public static void main(String[] args) {
      Productos Productos1 = new Productos("celular", 800000, 2, "xiaomi", "media");

        System.out.println(Productos1.getNombre());   
        System.out.println(Productos1.getPrecio());       
        System.out.println(Productos1.getCantidad());
        System.out.println(Productos1.getFabricante());
        System.out.println(Productos1.getCategoria());
        
        Productos1.setNombre("Smartphone");
         System.out.println(Productos1.getNombre());
 
        
    }
}






