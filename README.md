# ETAPA 4 AC1

Criei um produto e seus atributos com base no enunciado

## 🚀 Enunciados

Crie uma classe que representa um produto. Essa classe terá como atributos, nome, preço de custo, preço de venda, data de fabricação e data de validade.

Escreva construtores que recebem valores para inicializar seus atributos, onde:

1 - Recebe todos os atributos por parâmetro.

2 - Recebe o nome preço de custo, preço de venda e data de fabricação. Nesse caso a data de validade será 1 mês após a data de fabricação.

3 - Recebe apenas o nome e preço de custo. Nesse caso, o preço de venda será 10% a mais sobre o preço de custo e a data de validade segue o mesmo critério do item anterior.

### 📋 Códigos

public class Produto{
    private String nome;
    private double precoCusto;
    private double precoVenda;
    private String dataFabricacao;
    private String dataValidade;

  
    public Produto(String nome, double precoCusto, String dataFabricacao, String dataValidade) {  //Usei o metodo construtor que recebe todos os atributos por parâmetro; Construtor que recebe apenas nome e preço de custo; O preço de venda será 10% a mais sobre o preço de custo; E a data de validade será 1 mês após a data de fabricação
        this.nome = nome;
        this.precoCusto = precoCusto;
        this.precoVenda = precoCusto * 1.10;
        this.dataFabricacao = dataFabricacao;
        this.dataValidade = dataValidade;
    }



	public String getNome() {     //Utilizei o metodo getters e setters para acessar e modificar os atributos de forma mais controlada
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public double getPrecoCusto() {
        return precoCusto;
    }

    public void setPrecoCusto(double precoCusto) {
        this.precoCusto = precoCusto;
    }

    public double getPrecoVenda() {
        return precoVenda;
    }

    public void setPrecoVenda(double precoVenda) {
        this.precoVenda = precoVenda;
    }

    public String getDataFabricacao() {
        return dataFabricacao;
    }

    public void setDataFabricacao(String dataFabricacao) {
        this.dataFabricacao = dataFabricacao;
    }

    public String getDataValidade() {
        return dataValidade;
    }

    public void setDataValidade(String dataValidade) {
        this.dataValidade = dataValidade;
    }
    
    String descricao()  { //Na terceira etapa eu criei o retorno que vai ser o visual do código quando ele for gerado pelo aplicativo 
        return
            "Nome: " + this.nome + "\n" +
            "Preço de Custo: " + this.precoCusto+ "\n" +
            "Preço de Venda: " + this.precoVenda + "\n" +
            "Data de Fabricação: " + this.dataFabricacao + "\n" +
            "Data de validade: " + this.dataValidade + "\n";



     }
     public static void main (String[]args) {  //Por último criei o produto e pedi para o aplicativo printar para rodar
         Produto p1 = new Produto( "Bolo de Aniversário Personalizado do Todo Podero Timão", 89 , "9/11/2024", "09/12/2024");
      
         System.out.println(p1.descricao());
  
}
} 


### 🔧 Instalação

* Explicação de como deve ser utilizado o projeto

## 🛠️ Construído com

Ferramentas utilizadas e bibliotecas

* IDE Eclipse

## 📌 Versão

* **Versão 1.0** caso seja atualizado manter a descrição inicial e inserir uma nova linha com descrição da atualização.
* **Versão 1.1** - *Refatoração* *data 09/09/24*

## ✒️ Autores

João Carlos Ferreira de Araujo RA 248152 -- AC1 de Programação Orientada à Objetos

