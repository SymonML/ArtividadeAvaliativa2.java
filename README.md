# ArtividadeAvaliativa2.java

public class Empregado {
    private String nome;
    private String sobrenome;
    private double salarioMensal;

    public Empregado(String nome, String sobrenome, double salarioMensal) {
        this.nome = nome;
        this.sobrenome = sobrenome;
        this.salarioMensal = salarioMensal;
    }

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public String getSobrenome() {
        return sobrenome;
    }

    public void setSobrenome(String sobrenome) {
        this.sobrenome = sobrenome;
    }

    public double getSalarioMensal() {
        return salarioMensal;
    }

    public void setSalarioMensal(double salarioMensal) {
        this.salarioMensal = salarioMensal;
    }

    public double aumento() {
        double salarioAumentado = salarioMensal * 10 / 100; 
        return salarioAumentado;
    }

    public String toString() {
        return "Empregado: " + nome + " " + sobrenome + ", Salario Mensal: R$" + salarioMensal;
    }

    public static void main(String[] args) {
        Empregado empregado1 = new Empregado("Cleiton", "Jesus", 1500);
        Empregado empregado2 = new Empregado("Maria", "Fernanda", 3500);

        System.out.println(empregado1);
        System.out.println(empregado2);

        System.out.println("Aumento do salario de " + empregado1.getNome() + ": R$" + empregado1.aumento());
        System.out.println("Aumento do salario de " + empregado2.getNome() + ": R$" + empregado2.aumento());
    }
}
