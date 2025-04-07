Sistema de Gerenciamento de Medicamentos

Este é um sistema desktop desenvolvido em **JavaFX** que permite o gerenciamento de medicamentos e fornecedores em uma farmácia. Os dados são persistidos em arquivos CSV, garantindo facilidade e leveza na manipulação local.

Aplicação desenvolvida em JavaFX uqe permite o gerenciamento de medicamentos e fornecedores de uma farmacia, os dados sao armazenados em arquivos CSV.

 Funcionalidades

Cadastro de medicamentos
 Cadastro de fornecedores
 Pesquisa de medicamentos por código
Exclusão de medicamentos da tabela e do arquivo CSV
Relatórios:
Medicamentos controlados
  - Medicamentos com **estoque baixo**
  - Medicamentos **vencendo em até 30 dias**
- 💾 Dados salvos e carregados automaticamente do arquivo `medicamentos.csv`

## 💻 Tecnologias utilizadas

- **Java 17+**
- **JavaFX**
- **FXML (SceneBuilder)**
- **Java Collections / Streams**
- **Persistência em CSV**

## 🚀 Como executar o projeto

1. **Clone o repositório:**

```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
```

2. **Abra o projeto no IntelliJ, Eclipse ou outra IDE com suporte a JavaFX.**

3. **Configure o JavaFX** no seu ambiente, adicionando as bibliotecas do SDK.

   Exemplo de VM options (se necessário):

```
--module-path "caminho/para/javafx-sdk-XX.X.X/lib" --add-modules javafx.controls,javafx.fxml
```

4. Execute a aplicação a partir da classe `Main.java`.

## 📂 Estrutura de pastas

```
src/
├── main/
│   ├── java/
│   │   └── com/example/provan1/
│   │       ├── controller/
│   │       │   └── MainController.java
│   │       ├── model/
│   │       │   ├── Medicamento.java
│   │       │   └── Fornecedor.java
│   │       └── Main.java
│   └── resources/
│       └── com/example/provan1/
│           ├── MedicamentoView.fxml
│           ├── fornecedor.fxml
│           ├── Relatorio.fxml
├── datacsv/
│   └── medicamentos.csv
```

## ✅ Pré-requisitos

- JDK 17 ou superior
- JavaFX SDK (compatível com a sua versão de JDK)
- IDE (como IntelliJ IDEA ou Eclipse)
- SceneBuilder (opcional, mas recomendado para editar arquivos `.fxml`)

## 📝 Observações

- O arquivo `medicamentos.csv` deve existir na pasta `datacsv/` e conter os dados no seguinte formato:

```
codigo;nome;descricao;principioAtivo;dataValidade;quantidadeEstoque;preco;controlado;razaoSocialFornecedor;cnpjFornecedor
```

- O botão "Excluir Selecionado" remove o medicamento da tabela e atualiza o arquivo CSV automaticamente.
- Relatórios são gerados em janelas separadas com base em filtros aplicados.

## 📷 Capturas de tela (opcional)

> *(Adicione aqui imagens da interface, se desejar)*

## 🧠 Possibilidades futuras

- Integração com banco de dados (ex: PostgreSQL)
- Sistema de login
- Exportação de relatórios em PDF
- Filtros mais avançados de pesquisa

## 👨‍💻 Autor

Desenvolvido por [Seu Nome](https://github.com/seu-usuario)  
Curso: Engenharia de Software

## 📄 Licença

Este projeto é de uso livre para fins **educacionais** e não possui fins comerciais.
