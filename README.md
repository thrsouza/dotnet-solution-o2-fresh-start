# DOTNET SOLUTION CONFIGS

## 📦 Objetivo do Repositório

Este repositório foi criado para fornecer uma base padronizada que facilite a manutenção de boas práticas e o alinhamento entre equipes de desenvolvimento. Os arquivos aqui disponibilizados podem ser facilmente integrados em novos projetos ou adaptados para atender a necessidades específicas.

## 📋 Como Usar

1. Clone ou faça o download deste repositório.
2. Copie os arquivos desejados para a raiz do seu projeto.
3. Personalize as configurações, caso necessário, para atender a requisitos específicos.

## ⚙️ Arquivos de Configuração

### `.editorconfig`

O arquivo `.editorconfig` define padrões de formatação e estilo para diferentes linguagens de programação e configurações específicas para o editor. Exemplos:
- **Indentação**:
  - 4 espaços para a maioria dos arquivos.
  - 2 espaços para arquivos Markdown, JSON e YAML.
- **Estilo C#**:
  - Uso preferencial de tipos pré-definidos, como `int` em vez de `Int32`.
  - Controle do uso de `var` para tipos evidentes ou implícitos.
  - Padrões de nomenclatura:
    - Constantes e campos públicos: `PascalCase`.
    - Campos internos/privados: `_camelCase`.
  - Configurações de espaçamento e novas linhas para maior clareza no código.
- **Qualidade do Código**:
  - Supressão de diagnósticos redundantes, como [CA1032](https://learn.microsoft.com/pt-br/dotnet/fundamentals/code-analysis/quality-rules/ca1032) e [CS8602](https://learn.microsoft.com/pt-br/dotnet/csharp/language-reference/compiler-messages/nullable-warnings#possible-dereference-of-null).
  - Regras para namespaces baseados em escopo de arquivo.

### `.globalconfig`

O arquivo `.globalconfig` centraliza regras de estilo e qualidade que se aplicam globalmente ao projeto. Exemplos:
- **Regras de Estilo IDE**:
  - Avisos para simplificar inicializações de coleções e melhorar legibilidade.
  - Reforça práticas modernas, como o uso de operadores de índice e intervalos ([IDE0056](https://learn.microsoft.com/pt-br/dotnet/fundamentals/code-analysis/style-rules/ide0056) e [IDE0057](https://learn.microsoft.com/pt-br/dotnet/fundamentals/code-analysis/style-rules/ide0057)).
- **Supressão de Mensagens**:
  - Remove mensagens redundantes, como usings desnecessários e variáveis não utilizadas.
- **Qualidade do Código**:
  - Detecta problemas de clareza, como parênteses desnecessários ou instruções `switch` simplificáveis.
- Configurações modernas, como namespaces baseados em escopo de arquivo.

### `Directory.Build.Props`

O arquivo `Directory.Build.Props` define configurações de build compartilhadas entre todos os projetos no diretório:
- **Framework**: Define o framework-alvo como `.NET 9.0`, garantindo que os projetos estejam alinhados com as versões mais recentes e seus recursos.
- **Análise e Qualidade**: Habilita diagnósticos recomendados, tratando warnings como erros.
- **SonarAnalyzer**: Adiciona o analisador `SonarAnalyzer.CSharp` para fortalecer a análise estática de código.
- **Nullable**: Habilita a análise de referências nulas, aumentando a segurança e robustez do código.

---

Com esses arquivos, seu ambiente de desenvolvimento pode ser mais consistente e produtivo. 🚀
