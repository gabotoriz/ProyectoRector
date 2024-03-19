# Programación

Al momento de seleccionar un lenguaje de programación existian muchas opciones
* C
* C++
* Python

Sin ambargo se decidio por **JAVA** ya que siendo un lenguaje de facil nivel, es muy facil usar la abtracción que
requerimos para llevar las *Ecuaciones Diferenciales* a este lenguaje

## Herramientas utilizadas

* **Programacion (IDE)**
    * IntelliJ IDEA ULTIMATE
* **Documentacion**
    * WriterSide Jetbrains
* **Lenguaje De Programación**
    * JAVA
* **Librerias**
    * Lombok (Codigo Java mas limpio)

<tabs>
  <tab title="Java Vanilla">
<code-block lang="java">
public class Service {
    public static Service service;
    int IdServicio;
    String nombreServicio;
    String TipoDePlan;
    int Periodo;
    double PrecioReal;
    double PrecioVenta;
    int numeroDispositivos;
    int numeroPerfiles;
    public Service() {
    }
    public Service(int idServicio, String nombreServicio, String tipoDePlan, int periodo, double precioReal, double precioVenta, int numeroDispositivos, int numeroPerfiles) {
        IdServicio = idServicio;
        this.nombreServicio = nombreServicio;
        TipoDePlan = tipoDePlan;
        Periodo = periodo;
        PrecioReal = precioReal;
        PrecioVenta = precioVenta;
        this.numeroDispositivos = numeroDispositivos;
        this.numeroPerfiles = numeroPerfiles;
    }
    @Override
    public String toString() {
        return "Service{" +
                "IdServicio=" + IdServicio +
                ", nombreServicio='" + nombreServicio + '\'' +
                ", TipoDePlan='" + TipoDePlan + '\'' +
                ", Periodo=" + Periodo +
                ", PrecioReal=" + PrecioReal +
                ", PrecioVenta=" + PrecioVenta +
                ", numeroDispositivos=" + numeroDispositivos +
                ", numeroPerfiles=" + numeroPerfiles +
                '}';
    }
    public String getNombreServicio() {
        return nombreServicio;
    }
    public String getTipoDePlan() {
        return TipoDePlan;
    }
    public int getPeriodo() {
        return Periodo;
    }
    public double getPrecioReal() {
        return PrecioReal;
    }
    public double getPrecioVenta() {
        return PrecioVenta;
    }
    public int getNumeroDispositivos() {
        return numeroDispositivos;
    }
    public int getNumeroPerfiles() {
        return numeroPerfiles;
    }
    public static Service getService() {
        if (service == null) {
            service = new Service();
        }
        return service;
    }
}
</code-block>
  
  </tab>
  <tab title="Java Lambok">
  <code-block lang="java">
  @Getter
  @AllArgsConstructor
  @NoArgsConstructor
  @FieldDefaults(level = AccessLevel.PRIVATE)
  @ToString
  public class Client {
      public static Client cliente;
      int IdCliente;
      String Nombre;
      String ApePat;
      String ApeMat;
      String Correo;
      String Password;
      public static Client getCliente() {
          if (cliente == null) {
              cliente = new Client();
          }
          return cliente;
      }
  }
  </code-block>
  </tab>
</tabs>




