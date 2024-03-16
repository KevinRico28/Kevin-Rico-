public class LibrosDeTexto extends Libro{
    private String curso;
    
    

    public LibrosDeTexto(String titulo, String autor, String propietario, double precio, String curso) {
        super(titulo, autor, propietario, precio);
        //TODO Auto-generated constructor stub
        this.curso = curso;
    }

    public String getCurso() {
        return curso;
    }
    
    
    public void setCurso(String curso) {
        this.curso = curso;
    }
    





    public void ImprimirAqui(){
        super.imprimir();
        System.out.println("el curso es: " + curso);
    }

}

-------------------------------------------------------------------------------

public class Libro {
    protected String titulo;
    protected String autor;
    protected String propietario;
    protected double precio;
    
    public Libro(String titulo, String autor, String propietario, double precio) {
        this.titulo = titulo;
        this.autor = autor;
        this.propietario = propietario;
        this.precio = precio;
    }

    public String getTitulo() {
        return titulo;
    }

    public void setTitulo(String titulo) {
        this.titulo = titulo;
    }

    public String getAutor() {
        return autor;
    }

    public void setAutor(String autor) {
        this.autor = autor;
    }

    public String getPropietario() {
        return propietario;
    }

    public void setPropietario(String propietario) {
        this.propietario = propietario;
    }

    public double getPrecio() {
        return precio;
    }

    public void setPrecio(double precio) {
        this.precio = precio;
    }

    public void imprimir(){
        System.out.println("el titulo es: " + titulo );
        System.out.println(" el autor es: " + autor);
        System.out.println("el precio del libro es:  " + precio);
        
    }
}

-------------------------------------------------------------------------

public class LibroDeTextounijc extends LibrosDeTexto {
    private String facultad;

    public LibroDeTextounijc(String titulo, String autor, String propietario, double precio, String curso,String facultad) {
        super(titulo, autor, propietario, precio, curso);
        //TODO Auto-generated constructor stub
        this.facultad = facultad;
    }




    
    
    public void imprimirAqui(){
        super.imprimir();
        System.out.println("la facultad es: " + facultad);
    }
}

-------------------------------------------------------------------------

public class main {
    public static void main(String[] args) {
        
        Libro libroA = new Libro(titulo:null, autor:null, propietario:null, precio:0);
        libroA.setTitulo("Habitos Atomicos");
        libroA.setAutor("James Clear");
        libroA.setPropietario("Kevin Rico");
        libroA.setPrecio(48000);
        libroA.imprimir();
        
            
        LibrosDeTexto libroB = new Libro(titulo:null, autor:null, propietario:null, precio:0, curso:null);
        libroB.setTitulo("La importancia del no");
        libroB.setAutor("chris voss");
        libroB.setPropietario("Kevin Rico");
        libroB.setPrecio(65000);
        libroB.setCurso(C227);
        libroB.imprimir();


        LibrosDeTextouniajc libroC = new Libro(titulo:null, autor:null, propietario:null, precio:0, curso:null, facultad:null);
        libroC.setTitulo(titulo:" Griffonia ");
        libroC.setAutor(autor:"Michael Peinkofer ");
        libroC.setPropietario(propietario:"Kevin Rico");
        libroC.setPrecio(precio:50000);
        libroC.setfacultad(facultad:"ingenieria")
        libroC.imprimir();

        Novelas libroD = new Novelas(titulo:null, autor:null, propietario:null, precio:0, tipoNovelas:null);
        libroD.setTitulo(" naruto ");
        libroD.setAutor(" gideo ");
        libroD.setPropietario("Kevin Rico");
        libroD.setPrecio(73000);
        libroD.setTiposNovelas(" anime");
        libroD.imprimir();



    }

}

-------------------------------------------------------------------------------------

public class Novelas  extends LibroDeTextoInstitucion{
    private String tiposNovelas;

    public Novelas(String titulo, String autor, String propietario, double precio, String curso, String facultad, String tipoNovelas) {
        super(titulo, autor, propietario, precio, curso, facultad);
        //TODO Auto-generated constructor stub
        this.tiposNovelas = tipoNovelas;
    }


    public String getTiposNovelas() {
        return tiposNovelas;
    }

    public void setTiposNovelas(String tiposNovelas) {
        this.tiposNovelas = tiposNovelas;
    }

    public void imprimirAqui3(){
        super.imprimir();
        System.out.println(" el tipo de novela es: " + tiposNovelas);
    }

}
