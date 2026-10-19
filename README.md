Portal de Notícias - Fluxo Lista-Detalhe (Master-Detail)

Este projeto foi desenvolvido como parte da Aula 11 - Programação para Dispositivos Móveis I (Prof. Diego Menegassi). O objetivo principal é implementar a arquitetura de interface Master-Detail (Lista-Detalhe) integrada com o consumo de uma API REST e passagem de objetos fortemente tipados entre rotas no Flutter.

🎯 Objetivos do Projeto

Consumo de API REST: Integração com a API pública JSONPlaceholder para obtenção de dados assíncronos.

Padrão Master-Detail: Exibição inicial em uma lista e carregamento detalhado do item selecionado ao clicar no card.

Passagem de Objetos: Transferência da instância completa do NoticiaModel via Navigator.push e MaterialPageRoute.

Reutilização de Dados: Otimização de rede ao evitar chamadas adicionais para carregar informações que já foram obtidas na lista inicial.

📁 Estrutura de Pastas

lib/
├── models/
│   └── noticia_model.dart       # Modelo de dados e conversão factory de JSON
├── services/
│   └── noticia_service.dart     # Serviço HTTP de consumo da API REST
├── screens/
│   ├── feed_noticias_screen.dart # Tela principal com ListView.builder e FutureBuilder
│   └── detalhe_noticia_screen.dart # Tela de exibição dos detalhes da notícia
└── main.dart                     # Ponto de entrada da aplicação


🚀 Tecnologias e Pacotes Utilizados

Flutter SDK

Dart

Pacote http: Para requisições assíncronas no protocolo HTTP.

💻 Como Executar o Projeto

Clone este repositório:

git clone https://github.com/Lucascatto-z/pdm_aulall_master_detail
cd pdm_aulall_master_detail


Instale as dependências:

flutter pub get


Execute o aplicativo:

flutter run


📌 Histórico de Commits (Versionamento)

feat: cria modelo e servico HTTP com mapeamento completo de noticias

feat: implementa fluxo Master-Detail com Navigator push e telas de detalhes
