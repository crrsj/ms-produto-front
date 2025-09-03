🎨 Frontend de Produtos - Interface Web
📋 Descrição
Interface web moderna e responsiva para gerenciamento completo de produtos. Desenvolvida com HTML, CSS e JavaScript vanilla, integrada diretamente com a API de produtos.

🎯 Funcionalidades
📋 Listagem de Produtos - Visualização em tabela organizada

➕ Criação de Produtos - Formulário intuitivo para novos cadastros

✏️ Edição em Tempo Real - Atualização rápida de produtos existentes

🗑️ Exclusão Segura - Remoção com confirmação visual

🔍 Interface Responsiva - Adaptável a desktop e mobile

🔄 Atualização Automática - Sync em tempo real com a API

🏗️ Arquitetura Tecnológica
HTML5 - Estrutura semântica

CSS3 - Estilização moderna e responsiva

JavaScript ES6+ - Lógica e consumo de API

Fetch API - Comunicação RESTful

Design Responsivo - Mobile-first approach

🎨 Design & UX
Interface Limpa - Design minimalista e focado na usabilidade

Cores Profissionais - Palette azul corporativa com feedback visual

Animações Suaves - Transições e hover effects

Formulários Intuitivos - Validação e feedback imediato

Tabela Organizada - Layout claro para visualização de dados

📱 Layout & Componentes
Header Principal
html
<h1>Gerenciamento de Produtos</h1>
Formulário de Cadastro/Edição
Campos: Nome, Descrição, Preço, Estoque

Validação em tempo real

Botões: Salvar e Cancelar

Tabela de Produtos
Coluna	Descrição
ID	Identificador único
Nome	Nome do produto
Descrição	Detalhes do produto
Preço	Valor unitário (R$)
Estoque	Quantidade disponível
Ações	Editar/Excluir
⚡ Funcionalidades JavaScript
🔄 API Communication
javascript
const API_URL = 'http://localhost:8081/api/produtos';

// Operações disponíveis
async function loadProdutos()          // Carrega todos os produtos
async function createProduto(produto)  // Cria novo produto
async function updateProduto(id, produto) // Atualiza produto
async function deleteProduto(id)       // Remove produto
async function editProduto(id)         // Preenche formulário para edição
🎯 Event Handlers
Submit Form - Criação/atualização de produtos

Click Edit - Preenche formulário com dados existentes

Click Delete - Remove produto com confirmação

Click Cancel - Limpa formulário

🎨 Estilos CSS
Cores Principais
css
:root {
    --primary-color: #007bff;
    --success-color: #28a745;
    --danger-color: #dc3545;
    --light-color: #f8f9fa;
    --dark-color: #343a40;
}
Layout Responsivo
Desktop: Layout expandido com tabela completa

Tablet: Ajuste de tamanhos de fonte e padding

Mobile: Stack vertical e formulário otimizado

📊 Fluxo de Trabalho
1. 👀 Visualização
Carregamento automático ao abrir a página

Lista todos os produtos em tabela organizada

Informações: ID, Nome, Descrição, Preço, Estoque

2. ➕ Criação
Preenche formulário com dados do produto

Clique em "Salvar"

Atualização automática da tabela

Limpeza automática do formulário

3. ✏️ Edição
Clique em "Editar" em qualquer produto

Formulário preenchido automaticamente

Modifique os campos desejados

Clique em "Salvar" para atualizar

4. 🗑️ Exclusão
Clique em "Excluir" no produto desejado

Remoção imediata (sem confirmação popup)

Atualização automática da tabela

🚀 Acesso
URL do Frontend:

text
http://localhost:8081

