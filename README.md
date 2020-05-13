# heranca3-java
## Exercício pratico sobre Sobreposição, palavra super e anotação @Override

### Sobreposição ou sobrescrita
* É a implementação de um método de uma superclasse na subclasse

* É fortemente recomendável usar a anotação **@Override** em um método sobrescrito
  * Facilita a leitura e compreensão do código
  * Avisamos ao compilador(boa prática)
  
- **Método na classe Account**
```
public void withdraw(double amount){
  balance -= amount + 5.0;
}
```

- **Método da classe Account sobrescrita na classe SavingsAccount**
```
@Override
public void withdraw(double amount){
  balance -= amount;
}
```

### Palavra super
* É possível chamar a implementação da superclasse usando a palavra **super**.
```
@Override
public void withdraw(double amount){
  super.withdraw(amount);
  balance -= 2.0;
}
```
* A palavra **super** é também utilizada em construtores.

### Diagrama de classe:

![UML_Sobreposicao](https://github.com/glauberfernandes/heranca3-java/blob/master/UML_Sobreposicao.PNG)
