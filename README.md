# FastAPI Restaurantes API

Este é um projeto de API desenvolvido em FastAPI que fornece informações sobre os cardápios de restaurantes.

## Endpoints

### Hello World

- **Descrição**: Exibe uma mensagem incrível do mundo da programação!
- **URL**: `/api/hello`
- **Método HTTP**: GET
- **Exemplo de resposta**:
  ```json
  {
      "Hello": "World"
  }
Obter Cardápios de Restaurantes
Descrição: Retorna os cardápios dos restaurantes disponíveis.
URL: /api/restaurantes/
Método HTTP: GET
Parâmetros de consulta:
restaurante (opcional): Nome do restaurante para filtrar os resultados.
Exemplo de resposta (sem parâmetros de consulta):
json
Copy code
{
    "Dados": [ ... ]
}
Exemplo de resposta (com parâmetros de consulta):
json
Copy code

{
    "Restaurante": "Nome do Restaurante",
    "Cardapio": [
        {
            "item": "Nome do Item",
            "price": "Preço do Item",
            "description": "Descrição do Item"
        },
        ...
    ]
}

Execução Local
Para executar este projeto localmente, siga estas etapas:

Clone o repositório:

Copy code
git clone https://github.com/seu-usuario/fastapi-restaurantes-api.git
Instale as dependências:

Copy code
cd fastapi-restaurantes-api
pip install -r requirements.txt
Execute o servidor de desenvolvimento:

Copy code
uvicorn main:app --reload
Acesse a documentação da API em http://localhost:8000/docs.
Contribuição
Contribuições são bem-vindas! Se você deseja contribuir com este projeto, siga estas etapas:

Fork o projeto.
Crie uma branch para sua feature (git checkout -b feature/MinhaFeature).
Faça o commit das suas alterações (git commit -am 'Adicionando uma incrível nova feature').
Faça o push para a branch (git push origin feature/MinhaFeature).
Abra um Pull Request.

Licença
Este projeto está licenciado sob a Licença MIT - consulte o arquivo LICENSE para obter mais detalhes.
