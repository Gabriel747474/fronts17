Mini-projeto 1 – RESTful (Consumo de API Externa) Este projeto envolve uma página da web que utiliza a API OpenWeatherMap para fornecer dados meteorológicos, como temperatura, umidade e descrição do clima, para a cidade inserida pelo usuário. A função fetch foi usada para fazer a requisição, retornando os dados no formato JSON. Foi implementado o tratamento de erros para gerenciar casos como cidade não encontrada ou problemas de conexão, assegurando que o usuário receba uma mensagem compreensível em vez de a aplicação apenas falhar. Isso é fundamental para garantir a confiabilidade do aplicativo e proporcionar uma experiência positiva ao usuário.



Mini-projeto 2 – WebSockets (Interação em Tempo Real)
Este projeto cria um chat em tempo real, no qual as mensagens enviadas por um usuário são exibidas imediatamente para todos os demais usuários conectados.
A comunicação ocorreu por meio de WebSockets, que mantêm uma conexão bidirecional entre cliente e servidor.
Isso é mais eficaz do que o HTTP convencional, uma vez que elimina a necessidade de enviar requisições constantes (polling) para checar a presença de novas mensagens. Dessa forma, o sistema diminui o tráfego desnecessário e assegura uma experiência tranquila para o usuário.


Mini-projeto 3 – GraphQL (Consulta de Dados Eficiente)
A API pública Countries GraphQL foi empregada neste projeto para obter dados sobre países.
A consulta por escrito foi a seguinte:
consulta {
country(code: "BR") {
nome
capital
moeda
}
}
Essa consulta retorna apenas os campos essenciais (nome, capital e moeda) do país selecionado.
Ao contrário de uma requisição REST convencional, que pode retornar uma quantidade excessiva de dados irrelevantes, o GraphQL torna a consulta mais eficiente e econômica, fornecendo apenas as informações necessárias para a aplicação.
