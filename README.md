void main() {
  String nome = "Miguel F.";
  int idade = 20;
  double altura = 1.80;
  bool estudaFlutter = true;

  if (idade >= 18) {
    print("O aluno é maior de idade.");
  } else {
    print("O aluno é menor de idade.");
  }

  print(apresentarAluno(nome, idade, estudaFlutter));

  List<String> linguagens = ['JavaScript', 'Flutter', 'C'];
  Map<String, int> materias = {
    'POO': 40,
    'Estrutura de Dados': 35,
    'Banco de Dados': 25
  };

  print("Nome: $nome");
  print("Idade: $idade");
  print("Altura: $altura");
  print("Estudando Flutter: $estudaFlutter");
  print("Linguagens que gosto: $linguagens");
  print("Horas estudadas por matéria:");
  materias.forEach((materia, horas) {
    print("$materia: $horas horas");
  });
}

String apresentarAluno(String nome, int idade, bool estudaFlutter) {
  return "Olá, meu nome é $nome, tenho $idade anos e estou aprendendo Flutter: $estudaFlutter";
}
