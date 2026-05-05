## CENÁRIOS PRA FLUXO DE AQUISIÇÃO

### 1 - Pagamento Recusado:
Dado que usuario está na tela de pagamento
Quando ele inserir infomações inválidas do seu cartão 
Então o sistema deve exibir uma mensagem de erro e não concluir a compra

---

### 2 - Pagamento Aprovado:
Dado que o usúario está na tela de pagamento
Quando ele inserir informações válidas do seu cartão
Então o sistema deve exibir uma mensagem de aprovação e concluir a compra

---

### 3 - Cálculo de Frete:
Dado que o usúario inseriu um produto no seu carrinho
Quando ele informar o seu CEP válido
Então o sistema deve calcular e exibir valor de frete

---

### 4 - CEP Inválido:
Dado que o usuario está na tela de checkout
Quando ele informar o seu CEP Inválido
Então o sitema deve exibir mensagem de CEP inválido

---

### 5 - Carrinho inválido: 
Dado que o usúario está com o carrinho vazio
Quando ele tentar acessar o checkout 
Então o site não deve permitir ele continuar

---

### 6 - Cupom de Desconto:
Dado que o usúario possui um cupom de desconto
Quando ele aplicar um cupom válido
Então o site deve calcular o valor e aplicar o desconto

---

### 7 - Perguntas antes da Compra
Dado que o usúario está na aba de um produto
Quando ele não responder as perguntas necessárias para a compra
Então o site deve exibir os campos obrigatórios

---

### 8 - Login para Compra:
Dado que o usúario foi direcionado para a aba de checkout
Quando ele não ter login na página
Então o site deve exigir login antes da compra

---

### 9 - Sessão expirada:
Dado que usúario ficou inativo por muito tempo
Quando exceder o tempo de 15 minutos
Então o site deve perguntar se ele ainda permanece na página
