Em HTML, as instruções são chamadas de **tags** (ou elementos). Abaixo estão as principais tags divididas por categoria de uso:

---

### 1. Estrutura Básica do Documento

Todo documento HTML padrão começa com essa estrutura fundamental:

* `<!DOCTYPE html>`: Declara ao navegador que o documento usa a versão HTML5.
* `<html>`: Elemento raiz que envolve todo o conteúdo da página.
* `<head>`: Contém metadados, links para estilos externos e scripts (não visíveis diretamente na página).
* `<title>`: Define o título da aba do navegador.
* `<meta>`: Especifica informações como codificação de caracteres (`charset="UTF-8"`) ou configurações de tela/responsividade (`viewport`).
* `<link>`: Importa arquivos externos, como folhas de estilo CSS (`style.css`).
* `<body>`: Contém todo o conteúdo visual visível pelo usuário (textos, imagens, botões).

---

### 2. Cabeçalhos e Textos

Usados para hierarquia textual, parágrafos e ênfase:

* `<h1>` a `<h6>`: Títulos da página, onde `<h1>` tem o maior peso semântico e visual, e `<h6>` o menor.
* `<p>`: Define um parágrafo de texto.
* `<span>`: Contêiner genérico em linha (usado para estilizar trechos específicos de texto).
* `<strong>`: Indica texto com forte importância (visualmente em negrito por padrão).
* `<em>`: Indica ênfase textual (visualmente em itálico por padrão).
* `<br>`: Insere uma quebra de linha forçada.
* `<hr>`: Insere uma linha horizontal divisória.

---

### 3. Links e Mídias

Responsáveis por navegação e exibição de elementos visuais:

* `<a href="...">`: Cria um hiperlink para outra página, arquivo ou âncora interna.
* `<img src="..." alt="...">`: Exibe uma imagem (`src` é o caminho e `alt` é a descrição acessível).
* `<audio>` e `<video>`: Reproduzem mídias de áudio e vídeo diretamente no navegador.

---

### 4. Listas

Organizam itens sequenciais ou não sequenciais:

* `<ul>`: Lista não ordenada (com marcadores/pontos).
* `<ol>`: Lista ordenada (numerada alfabética ou numericamente).
* `<li>`: Cada item dentro de uma lista `<ul>` ou `<ol>`.

---

### 5. Estruturação Semântica

Introduzidas para melhorar a acessibilidade e indexação por mecanismos de busca (SEO):

* `<header>`: Cabeçalho da página ou de uma seção específica.
* `<nav>`: Bloco destinado a links de navegação.
* `<main>`: Conteúdo principal e exclusivo da página.
* `<section>`: Seção temática independente do conteúdo.
* `<article>`: Conteúdo autônomo (ex.: um post de blog ou notícia).
* `<aside>`: Conteúdo complementar lateral (ex.: barras laterais).
* `<footer>`: Rodapé da página (contatos, direitos autorais).
* `<div>`: Bloco genérico sem significado semântico, usado principalmente para estilização e layout via CSS.

---

### 6. Formulários e Entradas de Usuário

Permitem coletar dados enviados pelo visitante:

* `<form>`: Delimita o formulário e define o método de envio (GET, POST).
* `<input>`: Campo de entrada com diversos tipos (`type="text"`, `password`, `email`, `checkbox`, `radio`, `file`).
* `<textarea>`: Campo para inserção de texto longo com múltiplas linhas.
* `<button>`: Botão clicável para submissão ou ações via JavaScript.
* `<select>` e `<option>`: Criam menus suspensos (dropdowns).
* `<label>`: Rótulo de texto associado a um campo de entrada para acessibilidade.

---

### 7. Tabelas

Utilizadas para organizar dados bidimensionais:

* `<table>`: Define a tabela.
* `<tr>`: Linha da tabela (*table row*).
* `<th>`: Célula de cabeçalho (*table header*).
* `<td>`: Célula padrão de dados (*table data*).
