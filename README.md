# Alpha Prime Imóveis - Portal de Imóveis Premium

Uma plataforma moderna e profissional para gerenciar e exibir listagens de imóveis premium em **HTML, CSS e JavaScript puro**.

## ✨ Características

✅ **Logo e Branding** - Logo SVG customizável com nome da empresa
✅ **Listagem de Imóveis** - Grid responsivo com cards profissionais
✅ **Filtros Avançados** - Filtrar por tipo, preço, localização
✅ **Busca em Tempo Real** - Busca por título ou localização
✅ **Sistema de Favoritos** - Salvar imóveis com localStorage
✅ **Modal de Detalhes** - Visualizar informações completas
✅ **Galeria de Fotos** - Múltiplas imagens por imóvel
✅ **Página de Contato** - Formulário e informações de contato
✅ **Design Premium** - Cores gradientes e animações suaves
✅ **Totalmente Responsivo** - Mobile, tablet e desktop
✅ **Sem Dependências** - Apenas HTML, CSS e JavaScript puro

## 📁 Estrutura de Arquivos

```
alpha_prime/
├── index.html      # Estrutura HTML
├── styles.css      # Estilos CSS
├── script.js       # Funcionalidades JavaScript
├── data.js         # Dados de imóveis
├── logo.svg        # Logo da empresa
└── README.md       # Este arquivo
```

## 🚀 Como Usar

### 1. Abrir o Projeto

Simplesmente abra o arquivo `index.html` em um navegador:

```bash
# Windows
start index.html

# Mac
open index.html

# Linux
xdg-open index.html
```

Ou arraste o arquivo `index.html` para o navegador.

### 2. Estrutura de Dados

Os imóveis estão definidos em `data.js`. Cada imóvel tem:

```javascript
{
    id: 1,
    title: "Apartamento Luxo 3 Quartos - Vila Mariana",
    description: "Descrição do imóvel...",
    price: 500000,                          // Preço em reais
    propertyType: "Apartamento",            // Tipo de imóvel
    transactionType: "Venda",               // Venda ou Aluguel
    location: "Av. Paulista, 1000",        // Endereço
    city: "São Paulo",                      // Cidade
    state: "SP",                            // Estado
    bedrooms: 3,                            // Quartos
    bathrooms: 2,                           // Banheiros
    area: 120,                              // Área em m²
    badge: "Ótimo Preço",                  // Badge especial
    agent: "João Silva",                    // Nome do agente
    phone: "(11) 99999-1111",              // Telefone
    email: "joao@alphaprime.com",          // Email
    images: ["url1", "url2", ...],         // URLs das imagens
    features: ["Piscina", "Academia", ...] // Características
}
```

## 🎨 Customização

### Alterar Logo

Edite o arquivo `logo.svg` ou substitua o SVG em `index.html`:

```html
<svg width="50" height="50" viewBox="0 0 200 60" xmlns="http://www.w3.org/2000/svg">
    <!-- Seu SVG aqui -->
</svg>
```

### Alterar Nome e Tagline

Em `index.html`, procure por:

```html
<h1 class="company-name">Alpha Prime</h1>
<p class="company-tagline">Imóveis Premium</p>
```

### Alterar Cores

Em `styles.css`, modifique as variáveis CSS:

```css
:root {
    --primary-color: #0066cc;      /* Azul principal */
    --secondary-color: #00a8e8;    /* Azul secundário */
    --accent-color: #00d4ff;       /* Azul claro */
    --text-color: #333;            /* Texto */
    --light-text: #666;            /* Texto claro */
    --border-color: #ddd;          /* Bordas */
    --success-color: #28a745;      /* Sucesso */
    --danger-color: #dc3545;       /* Perigo */
    --bg-light: #f5f5f5;           /* Fundo claro */
    --bg-white: #ffffff;           /* Fundo branco */
}
```

### Alterar Informações de Contato

Em `index.html`, procure pela seção de contato:

```html
<div class="contact-card">
    <h3>📞 Telefone</h3>
    <p><a href="tel:+5511999999999">(11) 99999-9999</a></p>
</div>
```

## 📝 Adicionar Novos Imóveis

Edite `data.js` e adicione um novo objeto:

```javascript
{
    id: 9,
    title: "Seu novo imóvel",
    description: "Descrição...",
    price: 500000,
    propertyType: "Apartamento",
    transactionType: "Venda",
    location: "Endereço completo",
    city: "Cidade",
    state: "UF",
    bedrooms: 3,
    bathrooms: 2,
    area: 120,
    badge: null,
    agent: "Nome do Agente",
    phone: "(11) 99999-9999",
    email: "agente@email.com",
    images: ["https://url-da-imagem.jpg"],
    features: ["Feature 1", "Feature 2"]
}
```

## 💾 Sistema de Favoritos

Os favoritos são salvos no `localStorage`:

- ✅ Persistem após fechar o navegador
- ✅ Cada navegador tem seus próprios favoritos
- ✅ Sem necessidade de servidor

Para limpar favoritos:

```javascript
// No console do navegador (F12)
localStorage.removeItem('alphaprime_favorites');
location.reload();
```

## 📱 Responsividade

Funciona perfeitamente em:

- 📱 Smartphones (320px+)
- 📱 Tablets (768px+)
- 💻 Desktops (1200px+)

Breakpoints em `styles.css`:

```css
@media (max-width: 768px) { ... }
@media (max-width: 480px) { ... }
```

## 🔗 URLs de Imagens

As imagens usam URLs do Unsplash (gratuito). Para usar suas próprias:

1. Hospede em um servidor (Imgur, Cloudinary, etc)
2. Altere as URLs em `data.js`

Exemplo:

```javascript
images: [
    "https://seu-servidor.com/imagem1.jpg",
    "https://seu-servidor.com/imagem2.jpg"
]
```

## 🎯 Páginas Disponíveis

### Home
- Apresentação da empresa
- Chamada para ação (Comprar/Alugar)
- Features destacadas

### Imóveis
- Listagem com grid responsivo
- Filtros avançados
- Busca em tempo real
- Modal com detalhes completos

### Favoritos
- Listagem de imóveis salvos
- Gerenciamento de favoritos
- Persistência com localStorage

### Contato
- Informações da empresa
- Formulário de contato
- Links para redes sociais

## 🎨 Design Features

✨ **Gradientes Modernos** - Cores que combinam perfeitamente
✨ **Animações Suaves** - Transições elegantes
✨ **Sombras Profundas** - Efeito de profundidade
✨ **Tipografia Premium** - Fontes profissionais
✨ **Ícones Emoji** - Visuais intuitivos
✨ **Hover Effects** - Interatividade clara

## 🐛 Troubleshooting

### As imagens não aparecem
- Verifique as URLs em `data.js`
- Certifique-se que o servidor está acessível
- Use `onerror` para placeholder (já implementado)

### Os favoritos não salvam
- Verifique se localStorage está habilitado
- Tente limpar o cache do navegador
- Abra o console (F12) para ver erros

### Filtros não funcionam
- Verifique IDs dos elementos HTML
- Abra o console (F12) para procurar erros

## 📚 Estrutura HTML

```html
<header>          <!-- Logo, nome, navegação -->
<main>
  <section>       <!-- Home -->
  <section>       <!-- Listings -->
  <section>       <!-- Favoritos -->
  <section>       <!-- Contato -->
</main>
<footer>          <!-- Informações e links -->
<modal>           <!-- Detalhes do imóvel -->
```

## 🚀 Próximos Passos

Para expandir:

1. **Backend** - Adicionar Node.js + Express
2. **Banco de Dados** - Usar MySQL/MongoDB
3. **Autenticação** - Login para usuários
4. **Mapa** - Integrar Google Maps
5. **Admin** - Painel para gerenciar imóveis
6. **API** - Criar API para integração
7. **Notificações** - Alertas de novos imóveis
8. **Agendamento** - Sistema de visitas

## 📄 Licença

Livre para usar e modificar.

## 💬 Suporte

Para dúvidas, consulte este README ou modifique o código conforme necessário.

---

**Alpha Prime Imóveis - Sua melhor escolha em imóveis premium** ⭐

Desenvolvido com ❤️ usando HTML, CSS e JavaScript puro
