# 02quest Vault v4.1

**Banco de dados ultra-denso com criptografia AES-256 e compressao GZIP**

Criado por **Joaquim Pedro de Morais Filho**

---

## Sobre

O 02quest Vault e um sistema de armazenamento de dados client-side que utiliza compressao avancada (GZIP + Base36) e criptografia militar (AES-256-GCM) para criar links compactos e seguros contendo seus dados.

### Caracteristicas

- **Ultra-Density**: Compressao GZIP + sanitizacao inteligente de dados
- **Criptografia AES-256-GCM**: Protecao militar com PBKDF2 (100.000 iteracoes)
- **Protocolo Hibrido**: Dados salvos em LocalStorage + URL compartilhavel
- **Busca Inteligente**: Filtro vetorial em tempo real
- **Paginacao**: Suporte a grandes volumes de dados
- **Migracao Automatica**: Compativel com formatos V3 e anteriores

### Como Funciona

1. **Sanitizacao**: Telefones sao reduzidos a apenas digitos, IDs sao convertidos para Base36
2. **Compressao**: Dados JSON sao compactados via GZIP
3. **Serializacao**: Binario comprimido e convertido para Base64 na URL
4. **Criptografia** (opcional): Dados comprimidos sao criptografados com AES-256-GCM

## Uso

Abra o arquivo `index.html` em qualquer navegador moderno.

### Funcionalidades

| Acao | Descricao |
|------|-----------|
| **Novo (+)** | Cria um novo banco de dados vazio |
| **Salvar** | Adiciona um registro ao banco |
| **Criptografar** | Ativa criptografia AES-256 com senha |
| **Copiar Link** | Copia a URL contendo os dados comprimidos |
| **Info V4** | Exibe informacoes sobre a tecnologia |

## Tecnologias

- HTML5 / CSS3 / JavaScript ES6+
- Tailwind CSS
- Lucide Icons
- Web Crypto API (AES-256-GCM)
- CompressionStream API (GZIP)

## Licenca

MIT License - Joaquim Pedro de Morais Filho
