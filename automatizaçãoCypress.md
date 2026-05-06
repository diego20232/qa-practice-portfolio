
## Automatizando Formulário Hub de Leitura com Cypress

describe('Validando Dashboard', () => {
    
  beforeEach(() => {
    cy.visit('register.html')
  });
 

 it('Deve retornar', () => {
 
  // Criando variável que recebe uma função especifica de gerar números baseado em data e hora
  
  let email = `diego${Date.now()}@teste.com` 
  
  cy.get('#name').type('Diego Sampaio')
  
  cy.get('#email').type(email)
  
  cy.get('#phone').type('123456554')
  
  cy.get('#password').type('diego@123')
  
  cy.get('#confirm-password').type('diego@123')
  
  cy.get('#terms-agreement').check()
  
  cy.get('#register-btn').click()
  
  cy.url().should('include', 'dashboard')
    
 }); 
  
});

URL fonte está hospedada nas config do Cypress -> baseUrl: "http://localhost:3000/"
