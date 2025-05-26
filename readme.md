# Pokedex API

![Pokedex](https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/dream-world/25.svg)

## Sobre o Projeto

Este projeto é uma aplicação web que implementa uma Pokedex interativa, utilizando a [PokeAPI](https://pokeapi.co/) para obter dados sobre os Pokémon. A aplicação permite visualizar uma lista de Pokémon com suas respectivas informações, como número, nome, tipos e imagens.

A Pokedex é uma interface amigável e responsiva que possibilita aos usuários navegar por diferentes Pokémon, carregando mais itens conforme necessário através de um botão "Carregar Mais".

## Tecnologias Utilizadas

O projeto foi desenvolvido utilizando as seguintes tecnologias:

- **HTML5**: Estruturação semântica do conteúdo da página
- **CSS3**: Estilização da interface com design responsivo
- **JavaScript (ES6+)**: Manipulação do DOM e consumo de API
- **Fetch API**: Realização de requisições HTTP para a PokeAPI
- **Normalize.css**: Normalização de estilos entre navegadores
- **Google Fonts (Roboto)**: Tipografia consistente

## Estrutura do Projeto

```
pokedex-API/
│
└── src/
    ├── css/
    │   ├── global.css     # Estilos globais da aplicação
    │   └── pokedex.css    # Estilos específicos da Pokedex
    │
    ├── js/
    │   ├── main.js           # Script principal e manipulação do DOM
    │   ├── poke-api.js       # Funções para consumo da PokeAPI
    │   └── pokemon-model.js  # Modelo de dados para Pokémon
    │
    └── index.html        # Página principal da aplicação
```

## Funcionalidades

- **Listagem de Pokémon**: Exibe uma lista de Pokémon com suas informações básicas
- **Carregamento Paginado**: Permite carregar mais Pokémon através do botão "Carregar Mais"
- **Visualização de Detalhes**: Mostra informações detalhadas como número, nome, tipos e imagem
- **Design Responsivo**: Interface adaptável para diferentes tamanhos de tela
- **Tipagem Visual**: Exibição dos tipos de cada Pokémon com estilização específica

## Instalação e Execução

O projeto é uma aplicação web estática, sem necessidade de instalação de dependências ou configuração de ambiente. Para executá-lo localmente, siga os passos abaixo:

1. **Clone o repositório**

```bash
git clone https://github.com/joaogriquena/pokedex-API.git
```

2. **Navegue até o diretório do projeto**

```bash
cd pokedex-API
```

3. **Abra o arquivo index.html no navegador**

Você pode abrir o arquivo `src/index.html` diretamente no seu navegador preferido, ou utilizar uma extensão como Live Server no Visual Studio Code para servir os arquivos localmente.

## Como Usar

Ao abrir a aplicação, você verá uma lista inicial de Pokémon. Para carregar mais Pokémon, basta clicar no botão "Carregar Mais" no final da página. Cada card de Pokémon exibe:

- Número do Pokémon
- Nome
- Tipos (com cores específicas para cada tipo)
- Imagem do Pokémon

A aplicação é intuitiva e não requer configurações adicionais para uso.

## Implementação Técnica

### Consumo da API

A aplicação utiliza a PokeAPI para obter dados dos Pokémon. O arquivo `poke-api.js` contém as funções responsáveis por fazer as requisições e processar os dados recebidos:

- `getPokemons(offset, limit)`: Busca uma lista de Pokémon com paginação
- `getPokemonDetail(pokemon)`: Busca detalhes específicos de um Pokémon

### Modelo de Dados

O arquivo `pokemon-model.js` define a estrutura de dados utilizada para representar um Pokémon na aplicação, garantindo consistência nos dados exibidos.

### Interface e Interação

O arquivo `main.js` é responsável pela manipulação do DOM e interação com o usuário, incluindo:

- Renderização da lista de Pokémon
- Tratamento do evento de clique no botão "Carregar Mais"
- Conversão dos dados da API para o formato de exibição HTML

## Contribuição

Se você deseja contribuir com este projeto, siga os passos abaixo:

1. Faça um fork do repositório
2. Crie uma branch para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. Faça commit das suas alterações (`git commit -m 'Adiciona nova funcionalidade'`)
4. Faça push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

## Licença

Este projeto é distribuído sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## Contato

João Griquena - [GitHub](https://github.com/joaogriquena)

Link do Projeto: [https://github.com/joaogriquena/pokedex-API](https://github.com/joaogriquena/pokedex-API)

---

Desenvolvido com ❤️ por João Griquena
