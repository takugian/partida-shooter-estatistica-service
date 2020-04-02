# partida-shooter-estatistica-service
Serviço de estatísticas de uma partida de shooter

## Use Case
Eu, como GM, quero receber eventos de uma partida de shooter e gerar estatísticas;

## Eventos que devem ser captados:
* MATCH #X: FULANO_A killed FULANO_B using ITEM_X;
* MATCH #X: FULANO_A got a double kill/triple kill;
* MATCH #X: FULANO_A connected at 10:00:00;
* MATCH #X: FULANO_A disconnected at 12:00:00;
* MATCH #X: FULANO_A sent a message: XXX;

## Estatísticas que devem ser geradas:
* Ranking: número de matanças, número de mortes, número de double kills, número de triple kills, tempo de jogo;
* Quem matou mais;
* Quem morreu mais;

## Pré requisitos:
* Sprint Boot com as dependências: WEB, JPA e H2;
* Criar testes (unitários, serviços e e2e);
* Persitir as estatísticas em um ranking mundial de jogadores;
* Utilizar REST para receber os eventos;
* Utilizar REST para expor as estatísticas;

## Dicas:
* O serviço pode receber o evento, fazer os tratamentos e gerar as estatísticas;
* Persistam o que quiserem no banco de dados para facilitar;
* Deixe o código flexível, pois o jogo pode ser lançado em outros idiomas no futuro;
* Deixe o código flexível, pois mais estatísticas podem ser necesssárias no futuro;
* Deixe o código flexível, pois mais eventos podem ser gerados no futuro;



