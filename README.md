# Carrinho de Compras - Testes Unitários

Este projeto contém a implementação e a suíte de testes unitários automatizados para a função `calcularTotal` de um carrinho de compras, utilizando JavaScript e Jest.

---

## 🚀 Tecnologias Utilizadas

* **Node.js** - Ambiente de execução JavaScript
* **Jest** - Framework de testes em JavaScript

---

## 🛠️ Funcionalidades e Regras de Negócio

A função `calcularTotal` é responsável por processar os itens do carrinho e aplicar as seguintes regras:

* **Validação de Carrinho:** Lança um erro com a mensagem `"Carrinho inválido"` caso o carrinho esteja vazio ou possua itens com quantidade menor ou igual a zero.


* **Desconto por Cupom:** Aplica 10% de desconto sobre o subtotal ao utilizar o cupom `'PROMO10'`.


* **Cálculo de Frete:**
* **Frete Grátis:** Para compras com valor igual ou superior a R$ 100.


* **Frete Fixo:** Cobra R$ 15 para compras com valor inferior a R$ 100.




* **Arredondamento:** Formata o valor final para exatamente duas casas decimais.



---

## 🧪 Casos de Teste (Suíte de Testes)

Os testes cobrem os seguintes cenários:

* `CT-01`: Deve conceder frete grátis para compras de exatamente R$ 100.


* `CT-02`: Deve aplicar 10% de desconto com o cupom `PROMO10`.


* `CT-03`: Deve lançar erro se houver item com quantidade negativa ou zero.


* `CT-04`: Deve arredondar o valor final para duas casas decimais.


* `CT-05`: Deve lançar erro para carrinho vazio.


* `CT-06`: Deve cobrar frete de R$ 15 para compras abaixo de R$ 100.



---

## 📂 Estrutura do Projeto

```text
├── carrinho.js       # Implementação da lógica de cálculo
└── carrinho.test.js  # Suíte de testes automatizados (Jest)

```

---

## 🔧 Como Executar os Testes

1. **Instale as dependências:**
```bash
npm install

```


2. **Execute a suíte de testes:**
```bash
npm test

```
