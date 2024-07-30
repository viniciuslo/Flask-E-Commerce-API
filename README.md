# E-commerce API

Esta é uma API para um sistema de e-commerce construída com Flask.

## Pré-requisitos

- Python 3.6+
- Flask
- Flask-SQLAlchemy
- Flask-Login
- Flask-Cors
- Werkzeug

## Instalação

1. Clone o repositório:

    ```bash
    git clone <URL_do_repositório>
    cd <nome_do_repositório>
    ```

2. Crie um ambiente virtual:

    ```bash
    python3 -m venv meuenv
    ```

3. Ative o ambiente virtual:

    ```bash
    source meuenv/bin/activate
    ```

4. Instale as dependências:

    ```bash
    pip install -r requirements.txt
    ```

5. Execute a aplicação:

    ```bash
    python application.py
    ```

## Endpoints

A documentação completa dos endpoints pode ser encontrada no arquivo `swagger.yaml`.

- `/login` (POST): Realiza login
- `/logout` (POST): Realiza logout
- `/api/products` (GET): Retorna uma lista de produtos
- `/api/products/{product_id}` (GET): Retorna detalhes de um produto pelo ID
- `/api/products/add` (POST): Adiciona um novo produto
- `/api/products/update/{product_id}` (PUT): Atualiza um produto pelo ID
- `/api/products/delete/{product_id}` (DELETE): Deleta um produto pelo ID
- `/api/cart/add/{product_id}` (POST): Adiciona um item ao carrinho
- `/api/cart/remove/{item_id}` (DELETE): Remove um item do carrinho
- `/api/cart` (GET): Visualiza o conteúdo do carrinho
- `/api/cart/checkout` (POST): Finaliza a compra e limpa o carrinho


## Estrutura do Projeto

```
.
├── application.py
├── requirements.txt
├── swagger.yaml
└── README.md
```



## Contribuição

1. Fork este repositório.
2. Crie uma branch com a sua feature: `git checkout -b minha-feature`.
3. Commit suas mudanças: `git commit -m 'Adiciona minha feature'`.
4. Push para a branch: `git push origin minha-feature`.
5. Envie um Pull Request.

## Licença

Este projeto está licenciado sob a licença MIT.
