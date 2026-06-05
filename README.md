package br.senai.compras;

public class ItemLista {

    private String descricao;
    private Unidade unidade;
    private double quantidade;

    private double quantidadeComprada;
    private double precoUnitario;

    public ItemLista(String descricao,
                     Unidade unidade,
                     double quantidade) {
        this.descricao = descricao;
        this.unidade = unidade;
        this.quantidade = quantidade;
    }

    public String getDescricao() {
        return descricao;
    }

    public Unidade getUnidade() {
        return unidade;
    }

    public double getQuantidade() {
        return quantidade;
    }

    public double getQuantidadeComprada() {
        return quantidadeComprada;
    }

    public void setQuantidadeComprada(double quantidadeComprada) {
        this.quantidadeComprada = quantidadeComprada;
    }

    public double getPrecoUnitario() {
        return precoUnitario;
    }

    public void setPrecoUnitario(double precoUnitario) {
        this.precoUnitario = precoUnitario;
    }

    public double getTotal() {
        return quantidadeComprada * precoUnitario;
    }
}
