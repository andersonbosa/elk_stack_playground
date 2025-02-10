# Playground Elastic Stack

Este repositório contém um ambiente de testes para o **Elastic Stack** utilizando Docker. 

## Como Usar

Siga os passos abaixo para configurar e acessar o ambiente:

1. **Iniciar os Serviços**:
   ```bash
   docker-compose up
   ```
   Este comando irá inicializar o Elasticsearch, Kibana e Logstash.

2. **Gerar o Token de Inscrição**:
   Execute o script para gerar o token de inscrição do Kibana:
   ```bash
   ./create_enrollment_token.sh
   ```

3. **Acessar Kibana**:
   Abra seu navegador e vá para:
   ```
   http://0.0.0.0:5601
   ```
   Isso abrirá a interface do Kibana.

4. **Inserir o Token de Inscrição**:
   Na tela de login do Kibana, insira o token de inscrição gerado anteriormente.

5. **Login**:
   Faça o login usando as seguintes credenciais:
   - **Usuário**: `elastic`
   - **Senha**: (a senha configurada no seu `docker-compose.yml`)

## Observações
- Certifique-se de que o Docker e o Docker Compose estejam instalados em sua máquina antes de executar os comandos.
- Para encerrar os serviços, você pode usar `docker-compose down`.
