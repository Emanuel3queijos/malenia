
[Vídeo](https://www.youtube.com/watch?v=jhDUxynEQRI&t=51s)

---

## 1. Classes e Objetos

**Classe** = molde/template que define atributos (estado) e métodos (comportamento). **Objeto** = instância concreta de uma classe, criada em tempo de execução.

```java
class Animal {
    String nome;              // atributo (estado)
    void emitirSom() { ... }  // método (comportamento)
}

Animal cachorro = new Animal(); // objeto = instância
```

> 💡 **Pegadinha de prova:** classe é conceito (estrutura estática); objeto é a realização em memória (dinâmica, em tempo de execução). A FGV gosta de trocar essas definições entre si.

---

## 2. Encapsulamento

**Definição:** esconder os detalhes internos de implementação de uma classe, expondo apenas o necessário através de uma interface pública controlada.

- Atributos geralmente `private`
- Acesso controlado via métodos `public` (getters/setters)
- Objetivo: **proteger o estado interno** e reduzir acoplamento

```java
class ContaBancaria {
    private double saldo; // não pode ser acessado diretamente de fora

    public double getSaldo() { return saldo; }
    public void depositar(double valor) {
        if (valor > 0) saldo += valor; // regra de negócio protegida aqui dentro
    }
}
```

> 💡 **Por que importa na prova:** encapsulamento é o pilar mais ligado ao princípio **SRP** (Single Responsibility) e à proteção de invariantes — questões costumam testar se você entende que encapsulamento não é só "usar `private`", mas **controlar como o estado pode mudar**.

---

## 3. Herança

**Definição:** mecanismo que permite uma classe (subclasse/filha) reutilizar atributos e métodos de outra classe (superclasse/pai), criando uma relação **"é um"** (is-a).

```java
class Animal {
    void emitirSom() { System.out.println("Som genérico"); }
}
class Cachorro extends Animal {
    @Override
    void emitirSom() { System.out.println("Latido"); } // sobrescrita
}
```

- `Cachorro` **é um** `Animal` → relação de herança correta
- Java: herança simples de classe (só um pai), múltipla via **interfaces**

> ⚠️ **Cuidado com a prova:** herança mal usada quebra o **Princípio de Substituição de Liskov (LSP)** — isso já caiu diretamente na prova (questão do `Cachorro extends Animal`, gabarito: código estava **correto**, respeitava LSP). Ver seção de referência cruzada abaixo.

---

## 4. Polimorfismo

**Definição:** capacidade de um mesmo método/interface se comportar de formas diferentes dependendo do objeto que o executa.

### Tipos principais (cobre praticamente tudo que cai):

|Tipo|O que é|Exemplo|
|---|---|---|
|**Polimorfismo de sobrescrita** (overriding)|Subclasse redefine método herdado da superclasse|`Cachorro` redefine `emitirSom()`|
|**Polimorfismo de sobrecarga** (overloading)|Mesmo nome de método, assinaturas diferentes (parâmetros)|`somar(int, int)` e `somar(double, double)`|
|**Polimorfismo paramétrico** (generics)|Métodos/classes que trabalham com tipos genéricos|`List<T>`|
|**Polimorfismo em tempo de execução** (dynamic binding)|JVM decide qual método chamar em runtime, baseado no tipo real do objeto|`Animal a = new Cachorro(); a.emitirSom();` → chama versão de `Cachorro`|

```java
Animal a = new Cachorro(); // referência do tipo pai, objeto do tipo filho
a.emitirSom(); // imprime "Latido" — polimorfismo em ação
```

> 💡 **Regra de ouro pra prova:** o polimorfismo mais cobrado é o de **sobrescrita + binding dinâmico** — a ideia de que você pode tratar objetos de subclasses diferentes de forma uniforme através da referência da superclasse, e cada um vai se comportar do seu próprio jeito.

---

## 5. Os 4 Pilares — Resumo Rápido (tabela de revisão)

|Pilar|Pergunta-chave que resolve|Palavra-chave em Java|
|---|---|---|
|**Encapsulamento**|Como proteger o estado interno?|`private`, getters/setters|
|**Herança**|Como reaproveitar comportamento entre classes relacionadas?|`extends`|
|**Polimorfismo**|Como o mesmo método pode se comportar diferente conforme o objeto?|`@Override`, binding dinâmico|
|**Abstração** _(bônus — não citado no edital mas sustenta os outros 3)_|Como modelar só o que importa, escondendo complexidade?|classes abstratas, interfaces|

---

## 6. Referência cruzada com questões já resolvidas

- **[[SOLID]]** → questão sobre `Cachorro extends Animal` testou diretamente **Liskov Substitution Principle**, que é uma extensão direta do conceito de herança + polimorfismo bem aplicados (gabarito: **C** — código estava correto, `Cachorro` podia substituir `Animal` sem quebrar o programa).
- **[[UML]]** → diagrama de classes é a representação visual direta de herança (seta vazia), associação, composição.
- **[[Design Patterns]]** → muitos padrões (Strategy, Template Method, Factory) usam herança/polimorfismo como mecanismo-base.

---

## 7. Padrão de pegadinha da FGV nesse tema

Baseado nas questões já analisadas da prova, a banca costuma:

1. **Trocar definições entre os 4 pilares** (ex: descrever herança como se fosse polimorfismo)
2. **Testar herança + LSP juntos** — dar um código Java real com `extends`/`@Override` e perguntar se viola ou respeita Liskov
3. **Confundir sobrecarga com sobrescrita** (overloading x overriding) — são conceitos completamente diferentes e é fácil trocar os nomes

> ✅ **Checklist de domínio:** você está pronto nesse submódulo se conseguir, olhando pra qualquer código Java com `extends` e `@Override`, responder na hora: "isso é herança, polimorfismo, ou os dois? Está respeitando LSP?"

---

Quer que eu continue no mesmo padrão para o próximo submódulo, **SOLID**?