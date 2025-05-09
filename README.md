<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Gerenciador de Obrigações</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container">
    <header>
      <h1>Gerenciador de Obrigações</h1>
      <nav>
        <ul>
          <li><button id="tasks-tab">Tarefas</button></li>
          <li><button id="lists-tab">Minhas Listas</button></li>
          <li><button id="notes-tab">Notas</button></li>
        </ul>
      </nav>
    </header>

    <section id="tasks-section" class="section-content">
      <h2>Gerenciar Tarefas</h2>
      <form id="task-form">
        <input type="text" id="title" placeholder="Título da obrigação" required />
        <select id="category">
          <option value="Deus">Deus</option>
          <option value="Família">Família</option>
          <option value="Trabalho">Trabalho</option>
          <option value="Estudos">Estudos</option>
          <option value="Igreja">Igreja</option>
        </select>
        <select id="priority">
          <option value="Alta">Alta</option>
          <option value="Média">Média</option>
          <option value="Baixa">Baixa</option>
        </select>
        <button type="submit">Adicionar Tarefa</button>
      </form>
      <div class="filters">
        <select id="filter-category">
          <option value="">Todas as Categorias</option>
          <option value="Deus">Deus</option>
          <option value="Família">Família</option>
          <option value="Trabalho">Trabalho</option>
          <option value="Estudos">Estudos</option>
          <option value="Igreja">Igreja</option>
        </select>
        <select id="filter-priority">
          <option value="">Todas as Prioridades</option>
          <option value="Alta">Alta</option>
          <option value="Média">Média</option>
          <option value="Baixa">Baixa</option>
        </select>
        <select id="filter-status">
          <option value="">Todos os Status</option>
          <option value="A Fazer">A Fazer</option>
          <option value="Feito">Feito</option>
        </select>
      </div>
      <ul id="task-list"></ul>
    </section>

    <section id="lists-section" class="section-content">
      <h2>Minhas Listas</h2>
      <form id="list-form">
        <input type="text" id="list-title" placeholder="Nome da Lista" required />
        <button type="submit">Criar Lista</button>
      </form>
      <div id="lists-container"></div>
    </section>

    <section id="notes-section" class="section-content">
      <h2>Notas</h2>
      <form id="note-form">
        <textarea id="note-content" placeholder="Escreva sua nota..." required></textarea>
        <button type="submit">Adicionar Nota</button>
      </form>
      <ul id="notes-list"></ul>
    </section>
  </div>

  <script src="script.js"></script>
</body>
</html>
