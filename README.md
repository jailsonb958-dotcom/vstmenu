<div align="center">

# VST · Menu

### Uma experiência à mesa, do primeiro café ao último brinde.

[![HTML](https://img.shields.io/badge/HTML-estático-E76F51?style=flat-square&logo=html5&logoColor=white)](./Index.html)
[![CSS](https://img.shields.io/badge/CSS-responsivo-264653?style=flat-square&logo=css3&logoColor=white)](./style.css)
[![Idiomas](https://img.shields.io/badge/idiomas-4-2A6F5B?style=flat-square)](#idiomas)

</div>

---

Um cardápio digital leve e responsivo para apresentar as opções de **café da manhã, almoço e jantar**. A interface foi pensada para valorizar a leitura dos pratos em telas grandes e pequenas, com navegação simples e seletor de idioma.

## O que você encontra

- Navegação por refeição: café da manhã, almoço e jantar.
- Pratos organizados em entradas, principais e sobremesas.
- Fotos dos pratos e descrições no próprio cardápio.
- Interface adaptável para celular, tablet e desktop.
- Seletor de idioma e traduções disponíveis para parte do conteúdo.
- HTML, CSS e JavaScript sem frameworks ou etapa de compilação.

## Prévia visual

O projeto contém uma fotografia de prato em [`img/IMG-20251130-WA0042.jpg`](./img/IMG-20251130-WA0042.jpg). Abra o site localmente para explorar a experiência completa.

## Executar localmente

É possível abrir `Index.html` diretamente no navegador. Para servir a pasta localmente, use Python:

```bash
python3 -m http.server 8000
```

Depois, acesse [http://localhost:8000/Index.html](http://localhost:8000/Index.html).

## Estrutura do projeto

```text
.
├── Index.html   # conteúdo, dados do cardápio e comportamento
├── style.css    # identidade visual e layout responsivo
├── README.md    # documentação do projeto
└── img/         # fotografias e imagens dos pratos
```

## Como atualizar o cardápio

1. Abra `Index.html` e localize o objeto `menu` no script da página.
2. Edite ou adicione os itens na refeição e categoria correspondentes.
3. Informe `name`, `desc` e o caminho de `img` relativo à raiz, por exemplo:

   ```js
   { img: './img/meu-prato.jpg', name: 'Nome do prato', desc: 'Descrição do prato.' }
   ```

4. Coloque a imagem em `img/` e confira se o nome e a extensão coincidem exatamente.
5. Se houver tradução, atualize também `dishTranslations`.

Os nomes das categorias de almoço e jantar são definidos no HTML e atualizados pela função `applyLanguage`.

## Idiomas

O menu pode ser exibido em **português, inglês, francês e espanhol**. As traduções do conteúdo estão em `dishTranslations`; quando uma tradução específica não existe, o texto em português é usado como alternativa.

## Tecnologias

- HTML semântico
- CSS responsivo, animações discretas e suporte a preferência por movimento reduzido
- JavaScript nativo

---

<div align="center">

Feito para deixar cada escolha mais convidativa.

</div>
