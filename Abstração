package com.mycompany.prova

class Prova {
    private double notaAV1;
    private double notaAV2;

    public Prova(double notaAV1, double notaAV2) {
        this.notaAV1 = notaAV1;
        this.notaAV2 = notaAV2;
    }

    public double calcularMedia() {
        return (notaAV1 + notaAV2) / 2;
    }
}

class ProvaUCB {
    private Prova prova;

    public ProvaUCB(double notaAV1, double notaAV2) {
        prova = new Prova(notaAV1, notaAV2);
    }

    public boolean aprovado() {
        return prova.calcularMedia() >= 7;
    }
}

class ProvaFafifo {
    private Prova prova;

    public ProvaFafifo(double notaAV1, double notaAV2) {
        prova = new Prova(notaAV1, notaAV2);
    }

    public boolean aprovado() {
        return prova.calcularMedia() >= 6;
    }
}

public class Teste {
    public static void main(String[] args) {
        ProvaUCB provaUCB = new ProvaUCB(8, 6);
        System.out.println("Aprovado na UCB: " + provaUCB.aprovado());
        
        ProvaFafifo provaFafifo = new ProvaFafifo(5, 7);
        System.out.println("Aprovado na Fafifo: " + provaFafifo.aprovado());
    }
}
