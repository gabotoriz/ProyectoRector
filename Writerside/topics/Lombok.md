# Lombok

Al momento de que se comenzo a hacer el proyecto mas grande vimos que uno de los problemas fue que al momento de que
comenzará a hacerse mas grande el codigo, se comenzo a hacer mas dificil de entender.

Por se opto por usar [Lombok](https://projectlombok.org/features/), Lombok es una libreria que facilita el uso de
conceptos de programacion como SETTERS, GETTERS, CONSUCTORES VACIOS, CONTSTRUCTORES CON PARAMETROS, entre otros. Usando
notaciones como @Getter, para hacer los getters de todos los atributos de una clase

A continuacion tenemos un ejemplo de como se crearia una clase con Java nativo y usando Lambok

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