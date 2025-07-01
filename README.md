# 📁 Organizador de Arquivos do Google Drive

Este projeto implementa um **Organizador Automático de Arquivos** no Google Drive, utilizando Python. O objetivo é facilitar a organização de arquivos armazenados na nuvem, permitindo que sejam reorganizados com base em **tipo**, **data da última modificação**, **tamanho do arquivo** ou **palavras-chave** no nome. O código foi desenvolvido especialmente para ser executado no **Google Colab**, aproveitando sua praticidade na autenticação com o Google Drive e facilidade de uso.

A ferramenta foi criada como parte de uma contribuição em um projeto open-source e busca resolver um problema prático enfrentado por muitos usuários: **a dificuldade de manter o Drive organizado quando há grande volume de arquivos**.

## Estrutura do Projeto

- **`google_drive_organizer.ipynb`**: Notebook principal com todas as funções e instruções detalhada para o uso.

## Funcionalidades

1. **Organização por Tipo de Arquivo**:

   - Classifica arquivos com base em seu tipo (PDF, Documentos, Planilhas, etc.) e os move para subpastas correspondentes.

2. **Organização por Data**:

   - Agrupa os arquivos com base na data de modificação (ano/mês), útil para controle temporal de documentos.

3. **Organização por Tamanho**:

   - Distribui os arquivos em categorias como "Pequeno", "Médio", "Grande" e "Gigante", com base no tamanho em bytes.

4. **Organização por Palavras-chave**:

   - Identifica palavras-chave no nome do arquivo e cria subpastas temáticas automaticamente.

## Exemplo de Estrutura Gerada

```bash
Organizando por data de modificação:

├── 📁 Meu Drive/
│   │   ├── 📁 2024-06/                 
│   │   │   ├── 📄 reuniao.docx
│   │   │   └── 📄 foto.jpg
│   │
│   │   ├── 📁 2025-04/                 
│   │   │   ├── 📄 prova1.pdf
│   │   │   └── 📄 atividade.xlsx

```
## Observações

- A organização é feita sem apagar ou excluir nenhum arquivo.
- Se desejar aplicar mais de um critério, o ideal é fazer isso de forma planejada e manual, ou criar uma função personalizada que combine os critérios de forma hierárquica (por exemplo: tipo → data).
- Você pode (e deve) escolher uma **pasta específica** para organizar — e todas as **subpastas** serão incluídas automaticamente. Não é necessário aplicar as funções na raiz do seu Drive (`/MeuDrive`), a menos que deseje reorganizar absolutamente tudo.
- O projeto é ideal para quem usa o Google Drive de forma intensiva e precisa de uma estrutura de pastas automatizada.
- Todo o código foi escrito de forma enxuta e clara, com menos de 100 linhas de Python distribuídas em células funcionais.
- ⚠️ Embora seja tecnicamente possível executar duas ou mais funções de organização em sequência, **não é recomendado**. Isso porque cada função move os arquivos para uma estrutura diferente, o que pode desfazer a organização anterior.

---

                                 Projeto desenvolvido por Michel Alexandrino de Souza.
