## Teste de Cenário - Comgás Soluções

- Objetivo Central: Validar login com o método BDD 

### Cenário 1: Login Válido
Dado que usuário está na tela de login
Quando ele digitar credenciais válidas
Então ele deve acessar o sistema

---

### Cenário 2: Login Inválido
Dado que o usuário está na tela de login
Quando ele inserir o e-mail válido mas a senha inválida
Então ele não deve acessar o sistema

---

### Cenário 3: Login Inválido
Dado que o usuário está na tela de login
Quando ele inserir credenciais inválidas
Então ele não deve acessar o sistema

---


### Cenário 4: Redirecionando para recuperação de senha
Dado que o usuário digitou o login incorreto mais de 3 vezes
Quando ele tentar realizar o login pela 4ª vez
Então o sistema deve direcioná-lo para a página de recuperação de acesso



