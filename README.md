# Desafio

QUESTÃO 01
Scanner entrada = new Scanner(System.in);
List<String> degraus = new ArrayList<>();
System.out.print("Digite a quantidade de vezes: ");
int qtdDegraus = entrada.nextInt();
for (int i = 0; i < qtdDegraus; i++) {
degraus.add(" ".repeat(qtdDegraus - i) + "*".repeat(i + 1));
}
for (String d : degraus ) {
System.out.println(d);
}
                                                 
QUESTÃO 02
public class SenhaForte {
public static void main(String[] args) {
boolean invalido = true;
System.out.println("Introdução da senha requisito");
do {
System.out.print("Digite sua senha: ");
String senha = sc.next();
boolean valida = Pattern.matches("^(?=.*[a-z])(?=.*[A-Z])(?=.*\\d)(?=.*[-+_!@#$%^&*.,?])(?=.{6,}).+$",
senha);
if (valida == true) {
System.out.println("Senha forte cadastrada com requisitos atendidos no padrão!");
break;
} else {
valida = false;
System.out.println("Senha fraca! não atende ao requisitos mminimo pedidos");
}
} while (invalido);
}
}
                                                 
QUESTÃO 03
public class Anagrama {
public static void main(String[] args) {
Scanner scan = new Scanner(System.in);
System.out.println("ANAGRAMAS");
System.out.print("Informe a palavra: ");
String palavra = scan.nextLine();
numeroAnagaramas(palavra);
}
static void numeroAnagaramas(String palavra) {
if (palavra.charAt(i) == palavra.charAt(j) && i < j && i != j) {
if (palavra.charAt(i) == palavra.charAt(i + 1)) {
String x = palavra.substring(i, i + 1);
Anagramas.add(x);
else {
String y = palavra.substring(i, i + 1);
Anagramas.add(y);
String z = palavra.substring(i, j);
}
}
}
}
System.out.println(palavra.toUpperCase() + ": Contém " + "[" + Anagramas.size() + "]"
+ " pares de substrings que são anagramas.");
}
}                                                                                               
