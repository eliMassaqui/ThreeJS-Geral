# Guia Prático de Setup para Projetos 3D Web com Three.js

## Instalação das Dependências

```bash
npm install three@0.183.2 vite gsap cannon-es @dimforge/rapier3d socket.io-client lil-gui postprocessing three-stdlib howler gl-matrix three-ik
```

### Bibliotecas e Funções

| Biblioteca         | Função                         |
| ------------------ | ------------------------------ |
| three              | Renderização 3D                |
| vite               | Dev server e build             |
| gsap               | Sistema de animação            |
| cannon-es          | Motor de física alternativo    |
| @dimforge/rapier3d | Física moderna baseada em WASM |
| socket.io-client   | Comunicação em tempo real      |
| lil-gui            | Painel de parâmetros           |
| postprocessing     | Efeitos visuais                |
| three-stdlib       | Utilidades extras do Three.js  |
| howler             | Sistema de áudio               |
| gl-matrix          | Matemática vetorial e matrizes |
| three-ik           | Cinemática inversa             |

---

# Tecnologias e Ferramentas

* Three.js — Biblioteca 3D para Web
* Vite — Ferramenta moderna de build e dev server
* Node.js — Executar JavaScript fora do navegador
* NPM — Gerenciador de dependências

---

# Links Úteis

* [https://threejs.org/docs/](https://threejs.org/docs/)
* [https://vitejs.dev/](https://vitejs.dev/)
* [https://nodejs.org/](https://nodejs.org/)

---

# Configuração do Projeto

## 1. Criar um Projeto Node.js

```bash
mkdir threejs-project
cd threejs-project
npm init -y
```

## 2. Instalar Dependências Básicas

```bash
npm install vite three
```

## 3. Configurar Scripts no package.json

```json
"scripts": {
  "dev": "vite",
  "build": "vite build",
  "preview": "vite preview"
}
```

| Comando         | Função                             |
| --------------- | ---------------------------------- |
| npm run dev     | Inicia servidor de desenvolvimento |
| npm run build   | Gera build otimizado               |
| npm run preview | Visualiza build localmente         |

---

# Executar o Projeto

## Desenvolvimento

```bash
npm run dev
```

---

# Build para Produção

```bash
npm run build
```

O Vite irá gerar automaticamente a pasta:

```
dist/
```

Essa pasta contém os arquivos finais prontos para deploy.

---

# Testar o Build

```bash
npm run preview
```

---

# Rodar sem Node.js

Após gerar o build, o projeto pode ser executado em qualquer computador usando um servidor simples.

```bash
cd dist
python -m http.server 8000
```

Abrir no navegador:

```
http://localhost:8000
```

---

# Observação

Navegadores modernos bloqueiam módulos carregados via file://.

Sempre utilize um servidor local para rodar projetos Three.js com ES Modules.
