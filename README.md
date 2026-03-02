# Job Finder

Um gerador de URLs otimizadas para busca de vagas no LinkedIn, desenvolvido para facilitar a procura por oportunidades de trabalho com filtros específicos.

## Sobre o Projeto

O Job Finder é uma ferramenta web simples e eficiente que permite aos usuários configurar filtros de busca personalizados e gerar automaticamente URLs do LinkedIn Jobs com os parâmetros desejados. A aplicação foi desenvolvida com foco na experiência do usuário e na precisão dos resultados de busca.

## Funcionalidades

* **Busca por Cargo**: Digite qualquer posição ou função desejada
* **Filtro de Senioridade**: Selecione entre Estágio, Júnior, Pleno ou Sênior
* **Modalidade de Trabalho**: Escolha entre Presencial, Remoto ou Híbrido
* **Filtro Temporal**: Encontre vagas publicadas na última hora, 24 horas ou semana
* **Geração Automática de URL**: URL otimizada gerada automaticamente para o LinkedIn
* **Interface Responsiva**: Design adaptável para diferentes dispositivos

## Tecnologias Utilizadas

* HTML5
* CSS3
* JavaScript (Vanilla)
* Bootstrap 5.3.0
* Font Awesome 6.4.0

## Como Usar

1. Abra o arquivo `index.html` em seu navegador

2. Preencha os campos de acordo com sua busca:

   * **Cargo**: Digite a posição desejada (ex: "Desenvolvedor Frontend")
   * **Senioridade**: Selecione o nível de experiência (Todas, estágio, júnior, pleno, senior)
   * **Modalidade**: Escolha o formato de trabalho (todas, híbrido, remoto, presencial)
   * **Data do anúncio**: Filtre por tempo que a publicação está no ar (qualquer data, última hora, 24 horas, última semana)

3. Clique em "Buscar Vaga"

4. Uma nova aba será aberta com os resultados filtrados no LinkedIn

## Recursos Avançados

### Filtros de Exclusão

O sistema automaticamente adiciona filtros `NOT` para excluir níveis de senioridade não desejados, aumentando a precisão dos resultados.

### Mapeamento de Parâmetros

A aplicação converte os filtros selecionados nos parâmetros corretos da API do LinkedIn:

* Modalidades são convertidas para códigos específicos (Remoto: 2, Presencial: 1, Híbrido: 3)
* Filtros temporais são mapeados para valores de timestamp
* Termos de senioridade são padronizados

## Estrutura do Projeto

```
jobfinder/
│
├── index.html      # Arquivo principal da aplicação
├── README.md           # Documentação do projeto
```

## Instalação

Não há necessidade de instalação. Simplesmente:

1. Clone o repositório:

```bash
git clone https://github.com/rgiovann/jobfinder.git
```

2. Abra o arquivo `index.html` em qualquer navegador moderno

**Nota:** Para quem não tem familiaridade com o github, basta clicar no arquivo index.html, note então que você irá visualizar no canto superior direito um ícone de fazer download do arquivo. Se você ainda não conseguir identificar o ícone, passe o mouse sobre eles e perceba que em um dos ícones vai aparecer um "tooltip" com o texto "Download raw file". Salve o arquivo no seu computador e clique no mesmo que o browser irá automaticamente abrir a página.

## Compatibilidade

* Chrome 60+
* Firefox 55+
* Safari 12+
* Edge 79+

## Aviso Importante

O LinkedIn pode ignorar parcialmente filtros com `NOT` no campo de busca. Recomenda-se revisar os resultados manualmente para garantir a precisão das vagas encontradas.

## Nota 

Existe um segundo html, dedicado a procurar vagas nas PUBLICAÇÕES e não nas VAGAS, pois são oportunidades com menos visibilidade e portanto menos concorrência, apenas entre com as hashtags.

## Autor

**Giovanni L. Rozza**

* GitHub: [@rgiovann](https://github.com/rgiovann)

***

Desenvolvido com dedicação para facilitar a busca por oportunidades profissionais.
