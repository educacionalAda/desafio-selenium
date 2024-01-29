# Desafio técnico - Selenium

O objetivo deste desafio é desenvolver um conjunto de testes automatizados utilizando Selenium para o site de e-commerce fictício [https://www.saucedemo.com/](saucedemo.com), que simula um fluxo de compras online.

## Configurando o Ambiente

Para este desafio, você precisará ter o Java e o Selenium WebDriver configurados em seu ambiente de desenvolvimento. Também será necessário um navegador compatível com o WebDriver escolhido (por exemplo, ChromeDriver para Google Chrome).

## Desafio

Você deve criar um conjunto de testes automatizados seguindo os requisitos abaixo. Os testes devem ser implementados utilizando Selenium com Java.

## Requisitos

1. **Login:**
   - Automatizar o login no site saucedemo.com.
   - A senha para todos os usuários é "secret_sauce"

    - **Login com sucesso:**
        - Utilizando o usuário "standard_user", ao clicar no botão "Login" o acesso deverá ser realizado com sucesso.
    - **Login com usuário bloqueado:**
        - Utilizando o usuário "locked_out_user", ao clicar no botão "Login", deverá ser exibida uma mensagem informando o bloqueio.

2. **Acesso com erros**
    - Realizar login com o usuário "problem_user"
    - Os testes devem apontar erros como:
        - Imagens iguais
        - Ao adicionar um item, não é possível remover na tela inicial
        - Ao clicar nos detalhes de um produto, o detalhe exibido é de outro produto
        - Caso encontre algum outro erro e ache adequado, fique a vontade para incrementar os testes

3. **Navegação e Seleção de Produtos:**
    - Realizar login com o usuário "standard_user"
   - Automatizar a navegação pelas páginas de produtos.
   - Selecionar um ou mais produtos e adicioná-los ao carrinho de compras.

3. **Validação do Carrinho:**
    - Realizar login com o usuário "standard_user"
   - Automatizar a navegação até o carrinho de compras.
   - Verificar se os produtos selecionados estão no carrinho.

4. **Processo de Checkout:**
    - Realizar login com o usuário "standard_user"
   - Automatizar o preenchimento de informações de checkout (nome, sobrenome, código postal).
   - Finalizar a compra e validar a conclusão do pedido.

5. **Testes de Busca (se aplicável):**
- Realizar login com o usuário "standard_user"
   - Alterar ordenação dos produtos conforme o site permite
   - Verificar se os resultados correspondem à ordenação solicitada.

6. **Geração de Relatórios de Teste:**
   - Implementar a geração de relatórios detalhando os resultados dos testes, incluindo sucessos e falhas.

## Critérios de Avaliação

- **Qualidade do Código:** Código bem estruturado, organizado e comentado.
- **Cobertura de Testes:** Completude dos testes em relação aos requisitos.
- **Assertividade:** Precisão na verificação dos resultados esperados dos testes.
- **Tratamento de Exceções:** Capacidade de lidar com possíveis falhas ou variações no fluxo de testes.
- **Relatório de Testes:** Clareza e detalhamento nos relatórios gerados.

## Entrega

Os scripts de teste devem ser colocados em um repositório público no GitHub ou equivalente. Inclua um arquivo README.md com instruções detalhadas sobre como configurar o ambiente, executar os testes e quaisquer outras informações relevantes.

A entrega será a URL do repositório para avaliação.

## Diferenciais

- Uso de padrões de design de testes, como Page Object Model (POM).
- Testes bem documentados e com nomes claros.
- Implementação de testes adicionais além dos requisitos básicos.
- Uso de boas práticas de desenvolvimento, como DRY (Don't Repeat Yourself) e KISS (Keep It Simple, Stupid).
- Configuração para execução dos testes em diferentes navegadores.