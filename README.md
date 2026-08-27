# 🌻 PiMusic Sunflower

Servidor de streaming de arquivos MP3 com interface tema girassol, desenvolvido para Raspberry Pi 3 + PC Intel.

## 📋 Características

- ✅ **Streaming de áudio MP3** otimizado para Raspberry Pi
- ✅ **Galeria de álbuns** com capas com overlay escuro
- ✅ **Player de áudio** na sidebar direita (sticky)
- ✅ **Visualizador de letras** em formato TXT
- ✅ **Tema Girassol** com cores autênticas da planta
- ✅ **API REST** para comunicação Pi ↔ PC Intel
- ✅ **Upload via FileZilla**
- ✅ **Cloudflare Tunnel** para acesso seguro na internet

## 🏗️ Arquitetura

```
Raspberry Pi 3 (pimusic.com.br)
├── Nginx + PHP-FPM
├── Interface Web (Frontend)
└── Streaming de áudio

PC Intel (Backend)
├── Armazenamento 500GB
├── Processamento de áudio
└── Banco de dados da biblioteca

FileZilla ↔ Transferência de arquivos
```

## 🌍 Domínio

- **Principal**: pimusic.com.br
- **Acesso**: Cloudflare Tunnel

## ��� Estrutura do Projeto

```
PiMusic-Sunflower/
├── public/
│   ├── index.php
│   ├── css/
│   │   ├── sunflower-theme.css
│   │   └── player.css
│   ├── js/
│   │   ├── player.js
│   │   └── api.js
│   ├── assets/
│   │   └── images/
│   └── uploads/
│       └── album-covers/
├── api/
│   ├── albums.php
│   ├── tracks.php
│   ├── lyrics.php
│   └── stream.php
├── config/
│   ├── database.php
│   ├── paths.php
│   └── settings.php
├── nginx/
│   └── pimusic.conf
├── docker/
│   ├── Dockerfile.pi
│   └── docker-compose.yml
└── docs/
    ├── SETUP.md
    ├── API.md
    └── FILEMANAGEMENT.md
```

## 🚀 Quick Start

1. Clone o repositório
2. Configure as pastas em `config/paths.php`
3. Aponte seu domínio para o Nginx
4. Acesse `pimusic.com.br`

## 🎨 Paleta de Cores - Tema Girassol

- **Amarelo Principal**: #F4D03F
- **Amarelo Escuro**: #DAA520
- **Marrom Escuro**: #8B4513
- **Verde Folha**: #228B22
- **Fundo**: #FEF9E7
- **Texto Principal**: #2C1810

## 📝 Licença

MIT License

---

**Desenvolvido com ❤️ para pimusic.com.br**