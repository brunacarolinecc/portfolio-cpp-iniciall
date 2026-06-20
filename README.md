# portfolio-cpp-iniciall
Sistema simples em C++ para registro de estudantes, com uso de classes, encapsulamento e entrada/saída de dados. Projeto acadêmico para prática de programação orientada a #include <iostream>
using namespace std;

class Estudante {
private:
    string nome;
    int idade;

public:
    void setNome(string n) {
        nome = n;
    }

    void setIdade(int i) {
        idade = i;
    }

    string getNome() {
        return nome;
    }

    int getIdade() {
        return idade;
    }

    void exibirDados() {
        cout << "Nome: " << nome << endl;
        cout << "Idade: " << idade << endl;
    }
};

int main() {
    Estudante e;

    string nome;
    int idade;

    cout << "Digite o nome do estudante: ";
    getline(cin, nome);

    cout << "Digite a idade: ";
    cin >> idade;

    e.setNome(nome);
    e.setIdade(idade);

    cout << "\n--- Dados do Estudante ---" << endl;
    e.exibirDados();

    return 0;
}
