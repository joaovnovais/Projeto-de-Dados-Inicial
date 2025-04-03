## Sobre o Projeto

Este repositório é parte do workshop "Como Estruturar um Projeto de Dados do Zero". O objetivo principal é fornecer uma base sólida e uma estrutura padronizada para iniciar projetos de engenharia, ciência e análise de dados. A ideia é seguir boas práticas de desenvolvimento, automação, testes e documentação.

### Objetivos do Workshop:

* **Compreender a Estrutura de Projetos Padrão**: Aprender a organizar diretórios e arquivos, incluindo código-fonte, testes e documentação.

* **Melhores Práticas em Projetos de Dados**: Refatoração do projeto usando classes, módulos e boas práticas na implementação de uma ETL.

* **Explorar Ferramentas de Desenvolvimento**: Vamos discutir o uso de ambientes virtuais e ferramentas como PIP, CONDA e POETRY.

* **Testes com Pytest**: Implementar testes unitários e de integração para garantir que o código funcione conforme o esperado.

* **Controle de Versão com Git e GitHub**: Aprender a versionar seu projeto e colaborar com outras pessoas através do GitHub.

* **Documentação com MKDocs**: Documentar o projeto com MKDocs e publicar a documentação no [GitHub Pages](https://lvgalvao.github.io/DataProjectStarterKit/).

* **Automatização e CI/CD**: Configurar rotinas de Integração Contínua (CI) e Entrega Contínua (CD) para manter o projeto com qualidade alta durante todo o ciclo de vida.

## Começando

### Pré-requisitos

* **VSCode**: Usaremos o VSCode como editor de código durante o workshop. [Instruções de instalação do VSCode](https://code.visualstudio.com/download).

* **Git e GitHub**:

1. O Git precisa estar instalado em sua máquina. [Veja como instalar o Git aqui](https://git-scm.com/book/pt-br/v2).
2. Também é necessário ter uma conta no GitHub. [Instruções para criar sua conta no GitHub](https://docs.github.com/pt/get-started/onboarding/getting-started-with-your-github-account).
3. Se você for usuário Windows, recomendo este vídeo: [Youtube](https://www.youtube.com/watch?v=_hZf1teRFNg).
4. Tutorial básico de Git e Github [Ebook](https://www.linkedin.com/feed/update/urn:li:activity:7093915148351864832/?updateEntityUrn=urn%3Ali%3Afs_updateV2%3A%28urn%3Ali%3Aactivity%3A7093915148351864832%2CFEED_DETAIL%2CEMPTY%2CDEFAULT%2Cfalse%29&originTrackingId=4GUdvXH4TK%2BtZtlNHmiqJA%3D%3D).
5. Se você já sabe usar o Git, confira este vídeo do Akita: [Youtube](https://www.youtube.com/watch?v=6Czd1Yetaac).

* **Pyenv**: Para gerenciar as versões do Python. [Instruções de instalação do Pyenv](https://github.com/pyenv/pyenv#installation). Vamos usar a versão 3.11.3 para este projeto. Para Windows, assista a este tutorial [Youtube](https://www.youtube.com/watch?v=TkcqjLu1dgA).

* **Poetry**: Usaremos o Poetry para gerenciamento de dependências. [Instruções de instalação do Poetry](https://python-poetry.org/docs/#installation). Para Windows, recomendo este vídeo [Youtube](https://www.youtube.com/watch?v=BuepZYn1xT8), que também ensina a instalar Python, Poetry e VSCode. Caso prefira, um simples `pip install poetry` também resolve.

Sugestões de leitura:
- [Ebook 1 - Testes](https://www.linkedin.com/feed/update/urn:li:activity:7099722252144848896/?updateEntityUrn=urn%3Ali%3Afs_updateV2%3A%28urn%3Ali%3Aactivity%3A7099722252144848896%2CFEED_DETAIL%2CEMPTY%2CDEFAULT%2Cfalse%29&originTrackingId=hg1%2BufBeTLClrS%2BJixGEoA%3D%3D)
- [Ebook 2 - Github Actions](https://www.linkedin.com/feed/update/urn:li:activity:7098264928553201665/?updateEntityUrn=urn%3Ali%3Afs_updateV2%3A%28urn%3Ali%3Aactivity%3A7098264928553201665%2CFEED_DETAIL%2CEMPTY%2CDEFAULT%2Cfalse%29&originTrackingId=%2BFcdPRcDT62iNieFV3Yc%2Fg%3D%3D)
- [Ebook 3 - Na Minha Máquina Funciona](https://www.linkedin.com/feed/update/urn:li:activity:7095419109449814017/?updateEntityUrn=urn%3Ali%3Afs_updateV2%3A%28urn%3Ali%3Aactivity%3A7095419109449814017%2CFEED_DETAIL%2CEMPTY%2CDEFAULT%2Cfalse%29&originTrackingId=7ShpQeNCQuCDErI%2BAzEBXw%3D%3D)

### Instalação e Configuração

1. Clone o repositório:

```bash
git clone https://github.com/lvgalvao/dataprojectstarterkit.git
cd dataprojectstarterkit
```

2. Configure a versão do Python com o `pyenv`:

```bash
pyenv install 3.11.5
pyenv local 3.11.5
```

3. Configure o Poetry para usar a versão correta do Python e ative o ambiente virtual:

```bash
poetry env use 3.11.5
poetry shell
```

4. Instale as dependências do projeto:

```bash
poetry install
```

5. Execute os testes para garantir que tudo está funcionando:

```bash
task test
```

6. Execute o comando para acessar a documentação do projeto:

```bash
task doc
```

7. Execute o comando para rodar a pipeline de ETL:

```bash
task run
```

8. Verifique a pasta `data/output` para conferir se o arquivo foi gerado corretamente.
