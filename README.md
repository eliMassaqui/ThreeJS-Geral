# Guia Prático de Setup para Projetos 3D Web com Three.js

## Instalação das dependências

```bash
npm install three@0.183.2 vite gsap cannon-es @dimforge/rapier3d socket.io-client lil-gui postprocessing three-stdlib howler gl-matrix three-ik
```

| Biblioteca       | Função                       |
| ---------------- | ---------------------------- |
| Three.js         | renderização 3D              |
| vite             | dev server e build           |
| gsap             | animação                     |
| cannon-es        | física alternativa           |
| Rapier           | física moderna (WASM)        |
| socket.io-client | comunicação em tempo real    |
| lil-gui          | painel de parâmetros         |
| postprocessing   | efeitos visuais              |
| three-stdlib     | utilidades extras do Three   |
| howler           | áudio                        |
| gl-matrix        | matemática vetorial/matrizes |
| three-ik         | cinemática inversa           |


## Tecnologias e Ferramentas

- **Three.js** – Biblioteca 3D para web  
- **Vite** – Ferramenta de build rápida e moderna  
- **Node.js** – Executar JS fora do navegador  
- **NPM** – Gerenciador de dependências  

### Links Úteis
- [Documentação Three.js](https://threejs.org/docs/)
- [Vite.js](https://vitejs.dev/)
- [Node.js](https://nodejs.org/en/)

---

## Configuração do Projeto

### 1. Criar projeto Node.js
```bash
mkdir threejs-project
cd threejs-project
npm init -y

npm install vite three

npm run dev
```

Antes altere o package.joson pra os comandos de inicalizar e rodar o projecto no terminal:
```
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview"
  },
```
