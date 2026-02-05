# Jardim Pixel - Uma Experiência Interativa

![Preview](https://img.shields.io/badge/Status-Ativo-brightgreen) ![Pixi.js](https://img.shields.io/badge/Pixi.js-7.3.2-blue) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

Um jardim pixelizado interativo com física de grama, sistema de chuva, partículas e efeitos visuais dinâmicos. Clique e arraste para criar vagalumes e interagir com a grama!

## ✨ Funcionalidades Principais

### 🌿 Sistema de Grama Pixelizada
- **Geração procedural** de grama com cores gradientes
- **Física de oscilação** realista com influência do mouse
- **Cores customizáveis** (claro/escuro) via seletores
- **Sistema de chuva** com impacto visual na grama

### 🌦️ Sistema Climático Avançado
- **Chuva dinâmica** com intensidade, tamanho e velocidade ajustáveis
- **Efeito de vento** horizontal personalizável
- **Respingos e impacto** realistas
- **Molhamento progressivo** da grama

### 🎨 Sistema de Estações do Ano
- **4 estações predefinidas** (Primavera, Verão, Outono, Inverno)
- **Modo automático** que detecta a estação atual pela data
- **Cores temáticas** para cada estação
- **Troca manual** entre estações

### 💾 Sistema de Presets
- **Exportação/Importação** de configurações via JSON
- **Salvamento automático** no navegador (localStorage)
- **6 presets de performance** (Baixo → Ultra)
- **Presets temáticos** (Retro, Tempestade)

### ⚙️ Painel de Controle Completo
- **Interface deslizante** com animações suaves
- **Controles em tempo real** para todos os parâmetros
- **Estatísticas em tempo real** (FPS, contagem de objetos)
- **Relógio digital** flutuante com personalização completa

### ⚡ Otimização de Performance
- **Sistema de Chunks** para processamento por partes
- **Pooling de objetos** para partículas e efeitos
- **Cache de funções trigonométricas** para cálculos rápidos
- **Controles de densidade** para diferentes níveis de hardware

## 🚀 Como Usar

### Abrindo o Projeto
1. Salve o código como `index.html`
2. Abra o arquivo em qualquer navegador moderno
3. Não requer instalação ou servidor web

### Controles Básicos
- **Passe o mouse** sobre a grama para vê-la oscilar
- **Clique e arraste** para criar vagalumes
- **Botão ⚙️ no canto** para abrir o painel de configurações
- **Interaja com todos os controles deslizantes** no painel

### Sistema de Estações
1. **Modo Automático**: Ative o toggle "Modo Automático" para mudanças automáticas baseadas na data
2. **Modo Manual**: Clique em qualquer estação (Primavera, Verão, Outono, Inverno) para aplicar imediatamente
3. **Cores Customizadas**: Use os seletores de cor para criar seu próprio esquema

### Gerenciamento de Presets
- **Salvamento Automático**: Todas as configurações são salvas automaticamente
- **Exportar**: Clique em "Exportar Preset" para baixar um arquivo JSON
- **Importar**: Use "Importar Preset" para carregar configurações salvas
- **Presets de Performance**: Use os botões (Baixo, Médio, Alto, Ultra) para otimizar performance

## 🛠️ Tecnologias Utilizadas

- **Pixi.js 7.3.2**: Renderização 2D WebGL acelerada por hardware
- **HTML5 Canvas**: Para geração procedural de texturas
- **CSS3 Moderno**: Interface com animações e efeitos visuais
- **JavaScript ES6**: Lógica de simulação e interação

## 📊 Configurações Avançadas

### Otimização de Chunks
- **Tamanho do Chunk**: Controla a granularidade do processamento (8-64)
- **Chunks por Frame**: Quantos chunks são processados por frame (1-16)

### Sistema de Chuva
- **Intensidade**: Quantidade de gotas de chuva (10-100)
- **Tamanho**: Escala das gotas (0.5x-3x)
- **Velocidade**: Velocidade de queda (0.5x-2.5x)
- **Vento**: Força horizontal do vento (-5 a 5)
- **Impacto**: Força do impacto na grama (0.5x-3x)
- **Respingos**: Quantidade de partículas de respingo (0-10)

### Personalização Visual
- **Tamanho do Pixel**: Tamanho base dos pixels da grama (2-8px)
- **Densidade**: Percentual de cobertura da grama (10-100%)
- **Altura**: Altura máxima da grama (0.5x-2x)
- **Partículas de Fundo**: Quantidade de partículas estáticas (0-300)

## 🔧 Estrutura do Código

```
Jardim Pixel/
├── Renderização/
│   ├── Containers PIXI (background, grass, flowers, etc.)
│   ├── Sistema de texturas procedural
│   └── Sistema de pooling de objetos
├── Simulação/
│   ├── Física da grama (crescimento, oscilação, molhamento)
│   ├── Sistema de partículas (vagalumes, chuva, respingos)
│   └── Sistema de chunks para otimização
├── UI/
│   ├── Painel deslizante com controles
│   ├── Sistema de presets
│   └── Estatísticas em tempo real
└── Persistência/
    ├── Sistema de estações automáticas
    ├── Salvamento em localStorage
    └── Importação/Exportação JSON
```

## 🌐 Compatibilidade

- **Navegadores**: Chrome 90+, Firefox 88+, Safari 14+, Edge 90+
- **Dispositivos**: Desktop, Tablet, Mobile (com interface responsiva)
- **Requisitos**: GPU com suporte a WebGL (acelerado por hardware)

## 📱 Responsividade

- **Desktop**: Interface completa com painel lateral
- **Mobile**: Painel ocupa 100% da largura, botões otimizados
- **Toque**: Suporte completo a eventos touch

## 🔄 Atualizações Futuras (Planejadas)

- [ ] Adição de novas partículas (borboletas, pássaros)
- [ ] Sistema dia/noite com transição gradativa
- [ ] Mais presets de cores temáticas
- [ ] Sons ambientes (chuva, vento, insetos)
- [ ] Exportação de capturas de tela

## 📝 Licença

Este projeto está disponível para uso educacional e pessoal. Sinta-se à vontade para modificar e distribuir.

## 🐛 Reportando Problemas

Se encontrar algum bug ou tiver sugestões:
1. Verifique se está usando um navegador atualizado
2. Limpe o cache do navegador
3. Recarregue a página com Ctrl+F5
4. Problemas de performance: reduza a densidade ou use presets mais leves

---

**Criado com ❤️ usando Pixi.js** - Uma experiência relaxante de jardinagem pixelizada!
