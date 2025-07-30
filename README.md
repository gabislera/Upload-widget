# Upload Widget Web

Interface web responsiva para upload e gerenciamento de arquivos, construída com React, TypeScript e uma experiência de usuário moderna e interativa.

## Principais Tecnologias

- **React 19** + **TypeScript**
- **Vite** (build tool e dev server)
- **TailwindCSS** (estilização utilitária)
- **Zustand** (gerenciamento de estado)
- **Motion** (animações fluidas)
- **React Dropzone** (drag-and-drop de arquivos)
- **Radix UI** (componentes acessíveis)
- **Axios** (requisições HTTP)
- **Lucide React** (ícones)

## Funcionalidades

- **Upload Widget**: Interface compacta e expansível para upload de arquivos
- **Drag & Drop**: Arraste e solte arquivos diretamente na interface
- **Progress Tracking**: Acompanhamento visual do progresso de upload
- **Compressão de Imagens**: Otimização automática de imagens antes do envio
- **Lista de Uploads**: Visualização e gerenciamento dos arquivos enviados
- **Interface Responsiva**: Adaptada para diferentes tamanhos de tela
- **Animações Suaves**: Transições e feedback visual aprimorados


## Setup e Execução


### 1. Pré-requisitos

- Node.js 18+
- Servidor de upload rodando (https://github.com/gabislera/Upload-server)

### 2. Instalando dependências

```bash
npm install
```

### 3. Configuração do servidor

Certifique-se de que o servidor de upload esteja rodando na porta `3333` (ou ajuste a URL da API em `src/http/upload-file-to-storage.ts` se necessário).

### 4. Iniciando o servidor de desenvolvimento

```bash
npm run dev
```

A aplicação estará disponível em `http://localhost:5173`

### 5. Build para produção

```bash
npm run build
```

### 6. Preview da build de produção

```bash
npm run preview
```

### 7. Lint do código

```bash
npm run lint
```

## Estrutura do projeto

```
src/
├── components/           # Componentes React
│   ├── ui/              # Componentes base (botões, progress bar)
│   └── upload-widget-*   # Componentes específicos do widget
├── http/                # Camada de comunicação HTTP
├── store/               # Gerenciamento de estado (Zustand)
├── utils/               # Funções utilitárias
└── main.tsx             # Ponto de entrada da aplicação
```

## Observações

- O projeto utiliza Biome para lint/format, assim como o servidor
- As animações são otimizadas usando Motion (Framer Motion)
- A interface é totalmente responsiva e acessível
- O widget pode ser facilmente integrado em outras aplicações React