🚀 Projeto Apache com Docker Compose
Este projeto demonstra como utilizar o Docker Compose para configurar um servidor Apache simples que exibe uma página de sucesso. É ideal para quem está começando com Docker e deseja entender como servir páginas web estáticas com o Apache HTTP Server.
📦 Estrutura do Projeto
.
├── docker-compose.yml
└── website/
    └── index.html


- docker-compose.yml: Define o serviço Apache usando a imagem oficial httpd.
- website/: Diretório local que contém os arquivos HTML que serão servidos pelo Apache. Certifique-se de que o arquivo index.html esteja presente aqui.
🛠️ Como Executar
- Clone este repositório:
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
- Certifique-se de que o Docker e o Docker Compose estão instalados.
- Execute o serviço:
docker-compose up
- Acesse a página de sucesso no navegador:
http://localhost


🧰 Detalhes Técnicos
- Imagem utilizada: httpd:latest
- Porta exposta: 80
- Volume montado: O conteúdo da pasta ./website é servido diretamente pelo Apache em /usr/local/apache2/htdocs.
✅ Resultado Esperado
Ao acessar http://localhost, você verá a página definida em website/index.html, confirmando que o servidor Apache está funcionando corretamente via Docker Compose.
📄 Licença
Este projeto está sobre a licença MIT.
