# Exercicio-8-em-Java
# Exercicio replicado do livro Tutorial de programação em Java e Orientação a Objetos

# CONSTRUTORES E AGREGAÇÃO

Este exemplo é o resultado do exercício anterior (exercício 4 tópico “CONSTRUTORES”), ele
cria uma classe Reta com dois atributos da classe Ponto. Ou seja você estará reutilizando a classe
Ponto na classe que representa uma Reta, a forma como essa reutilização de código ocorre é
chamada de agregação.

//Reutilize o arquivo da classe Ponto definida anteriormente.
//Classe Reta
class Reta {
public Ponto a,b;
public Reta(float ax, float ay, float bx, float by) //construtor com argumentos
{
a = new Ponto(ax, ay); //chamadas dos contrutores da classe Ponto
 b = new Ponto(bx, by);
}
public void mostra()
{
 a.mostra();
 b.mostra();
}
}
//Classe principal, Arquivo Principal.java
class Principal {
 public static void main(String args[]) {
 Reta ar;
 ar=new Reta((float)0.0,(float)0.0,(float)1.0,(float)1.0);
 ar.mostra();
 }
}

# Argumento
Alguns podem argumentar que esta maneira de representar uma reta não é muito eficiente, mas
não é do escopo deste texto tratar de problemas dessa natureza, o que aliás complicaria muito o
código, desviando-nos do objetivo principal: simplicidade na apresentação de conceitos de orientação
a objetos. O leitor deve ampliar os modelos aqui sugeridos em aplicações na sua área de interesse.
Como ainda faltam conceitos importantes para serem apresentados este tipo de aplicação deve ser
feita em paralelo com a leitura.
