# 📦 dotnet-solution-o2-fresh-start

**Fresh Start para projetos em .NET Core**
Este repositório é um _template_ inicializado para criar novas soluções .NET de forma limpa, padronizada e preparada para desenvolvimento profissional.

---

## 📂 Estrutura Inicial

O repositório é iniciado com os seguintes arquivos e configurações:

- **Solution.slnx:** Estrutura modular baseada em diretórios, já preparada para organizar _Solution Items_ e projetos em `./src/`.
- **.editorconfig:** Padrões de formatação e estilo de código aplicáveis a todo o repositório.
- **.globalconfig:** Configurações globais do analisador de código C#.
- **.gitignore:** Padrão oficial para projetos .NET (ignora binários, obj, configurações locais, etc).
- **Directory.Build.Props:** Centraliza configurações MSBuild para toda a solução.

---

## ⚙️ Configurações do `Directory.Build.Props`

O arquivo `Directory.Build.Props` já inclui boas práticas recomendadas para novos projetos .NET:

- **Target Framework**: `net9.0`
- **Usings implícitos**: `enable`
- **Nullable Reference Types**: `enable`
- **Análise de Código**:
  - Nível: `latest`
  - Modo: `Recommended`
  - _Warnings_ tratados como erros
  - _CodeStyle_ validado em tempo de build
- **Analisador Adicional**:
  - `SonarAnalyzer.CSharp` (v10.8.0.113526)

---

## 🧩 Conteúdo da Solution

A solução `.slnx` já define a seguinte estrutura:

```xml
<Solution>
  <Folder Name="/Solution Items/">
    <File Path=".editorconfig" />
    <File Path=".gitignore" />
    <File Path=".globalconfig" />
    <File Path="Directory.Build.Props" />
    <File Path="LICENSE" />
    <File Path="README.md" />
  </Folder>
  <Folder Name="/src/" />
</Solution>
```

- `Solution Items`: Centraliza arquivos de configuração importantes.
- `src`: Diretório reservado para novos projetos e módulos da solução.

## 🚀 Como usar

1. Clone o repositório:
```bash
git clone https://github.com/thrsouza/dotnet-solution-o2-fresh-start.git
```
2. Abra a solução no Visual Studio ou Rider.
3. Adicione seus projetos dentro da pasta `/src/`.
4. Aproveite uma solução pronta para escalar com qualidade!

## 🛠️ Motivação

Esse repositório foi criado para acelerar a criação de novos projetos .NET, garantindo que todos partam de um padrão de qualidade e organização desde o início.

## 📜 Licença

Este projeto está licenciado sob a [MIT License](./LICENSE).
