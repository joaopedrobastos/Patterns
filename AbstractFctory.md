//interface para fábricas de carros

public interface FabricaDeCarro {

    //fábrica de carros sedan
    
    CarroSedan criarCarroSedan();
    
    //fábrica de carros populares
    
    CarroPopular criarCarroPopular();
}

//fábrica concreta

public class FabricaFiat implements FabricaDeCarro {

    //Todas fábricas concretas criam carros sedan e populares
    
    @Override
    public CarroSedan criarCarroSedan() {
        return new Siena();
    }
 
    @Override
    public CarroPopular criarCarroPopular() {
        return new Palio();
    }
 
}

