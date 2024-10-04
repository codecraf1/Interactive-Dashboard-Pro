# Interactive Dashboard Pro

Interactive Dashboard Pro é um projeto inovador desenvolvido exclusivamente com HTML e CSS, projetado para fornecer uma interface de usuário intuitiva e responsiva para visualização de dados e informações essenciais.

## Objetivos do Projeto

- **Interface Responsiva**: Garantir uma experiência de usuário perfeita em dispositivos de diversos tamanhos, desde desktops até smartphones.
- **Design Moderno**: Aplicar um design limpo e moderno, utilizando uma paleta de cores consistente, tipografia adequada e ícones personalizados.
- **Organização Eficiente**: Utilizar CSS Grid para uma organização clara e eficiente dos componentes do dashboard, facilitando a navegação e a acessibilidade das informações.
- **Interatividade Visual**: Incorporar animações e transições CSS para uma experiência de usuário mais envolvente e dinâmica.
- **Visualização de Dados**: Criar gráficos simples, como barras e linhas, utilizando apenas HTML e CSS, demonstrando o poder dessas tecnologias sem a necessidade de JavaScript.

## Componentes do Dashboard

- **Cabeçalho**: Inclui o título do dashboard e um menu de navegação.
- **Barra Lateral**: Oferece links rápidos para diferentes seções do dashboard, como perfil, notificações e mensagens.
- **Conteúdo Principal**: Contém seções como visão geral, análises e configurações, cada uma com cartões informativos e gráficos interativos.

## Estrutura do Projeto

### HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Dashboard</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="dashboard">
        <header class="dashboard-header">
            <h1>Dashboard</h1>
            <nav>
                <ul>
                    <li><a href="#overview">Overview</a></li>
                    <li><a href="#analytics">Analytics</a></li>
                    <li><a href="#settings">Settings</a></li>
                </ul>
            </nav>
        </header>
        <aside class="dashboard-sidebar">
            <ul>
                <li><a href="#profile">Profile</a></li>
                <li><a href="#notifications">Notifications</a></li>
                <li><a href="#messages">Messages</a></li>
            </ul>
        </aside>
        <main class="dashboard-content">
            <section id="overview">
                <h2>Overview</h2>
                <div class="card">
                    <h3>Total Users</h3>
                    <p>1,234</p>
                </div>
                <div class="card">
                    <h3>Sales</h3>
                    <p>$12,345</p>
                </div>
            </section>
            <section id="analytics">
                <h2>Analytics</h2>
                <div class="chart"> <!-- Placeholder for a CSS-only chart -->
                    <div class="bar" style="height: 50%"></div>
                    <div class="bar" style="height: 75%"></div>
                    <div class="bar" style="height: 60%"></div>
                </div>
            </section>
            <section id="settings">
                <h2>Settings</h2>
                <p>Settings content goes here...</p>
            </section>
        </main>
    </div>
</body>
</html>

### CSS

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #f0f2f5;
}

.dashboard {
    display: grid;
    grid-template-areas: 
        "header header"
        "sidebar content";
    grid-template-columns: 250px 1fr;
    grid-template-rows: auto 1fr;
    width: 80%;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.dashboard-header {
    grid-area: header;
    background-color: #333;
    color: #fff;
    padding: 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.dashboard-header nav ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    gap: 1rem;
}

.dashboard-header nav a {
    color: #fff;
    text-decoration: none;
}

.dashboard-sidebar {
    grid-area: sidebar;
    background-color: #444;
    color: #fff;
    padding: 1rem;
}

.dashboard-sidebar ul {
    list-style: none;
    margin: 0;
    padding: 0;
}

.dashboard-sidebar a {
    color: #fff;
    text-decoration: none;
    display: block;
    padding: 0.5rem 0;
}

.dashboard-content {
    grid-area: content;
    padding: 2rem;
    overflow-y: auto;
}

.card {
    background-color: #e7e7e7;
    padding: 1rem;
    margin-bottom: 1rem;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.chart {
    display: flex;
    gap: 1rem;
}

.bar {
    width: 20px;
    background-color: #007bff;
}

@media (max-width: 768px) {
    .dashboard {
        grid-template-areas: 
            "header"
            "content"
            "sidebar";
        grid-template-columns: 1fr;
        grid-template-rows: auto 1fr auto;
    }
}

Como Executar

	1.	Clone o repositório:

git clone https://github.com/seu-usuario/interactive-dashboard-pro.git


	2.	Navegue até o diretório do projeto:

cd interactive-dashboard-pro


	3.	Abra o arquivo index.html no seu navegador preferido.

Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests para melhorar este projeto.

Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

