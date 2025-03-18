# Spring---Annotations

<h3>@Qualifier("name")</h3>
<p>@Qualifier helps in injecting specific beans when there are multiple candidates of same type, is used to resolve ambiguity in these candidates. Below are some examples:</p>

<h3>Scenario 1: Multiple Beans of the Same Type:</h3>

<p>Below, the interface Animal with the deal for the all classes that implements animal use this:</p>

```java
  public interface Animal {

    String sound();
}

```
Below, two classes that implement the interface Animal

```java
  public class Cat implements Animal{

    @Override
    public String sound() {
        return "Meow";
    }
}

@Component
public class Dog implements Animal {

    @Override
    public String sound() {
        return "Bark";
    }
}

```



