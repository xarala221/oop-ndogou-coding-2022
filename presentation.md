# La programmation Orientée Objet

## Sommaire

- La programmation Orientée Objet
- La programmation Oreinté Objet en Python
- La programmation Oreinté Objet en Python et Java

## Présentation

Je m'appelle **Ousseynou DIOP** , fondateur de Xarala et Consultant-Formateur

- Ouicarry
- Volkeno
- Mentor Openclassrooms
- CasaCloud
- DataConsumed

## Les Paradigmes de programmation

Le paradigme de programmation est la façon (parmi d'autres) d'approcher la programmation informatique et de formuler les solutions aux problèmes et leur formalisation dans un langage de programmation approprié[Wikipedia](<https://fr.wikipedia.org/wiki/Paradigme_(programmation)>)

- Programmation procédurale
- Programmation événementielle
- Programmation Orientée Objet

## Historique de la programmation Orientée Objet

Le paradigme de programmation qu’est la POO a été défini par les norvégiens Ole-Johan Dahl et Kristen Nygaard au début de la décennie 1960

## Principes

- Encapsulation
- Héritage
- Polymorphisme

## Mots clés à comprendre

- Class
- Objet
- Attribut
- Méthode / Fonction
- Instanciation

## Application en Python

- Création de class

```python
class Car:
  pass
```

- Instanciation

```python
Car()

c1 = Car()
c2 = Car()

# si vous comparez les deux, vous aurez deux resultats different
```

```python
c1 == c2
False
```

- Attributs

```python
class Car:
  wheels = 12 # Attribut de classe
  def __init__(self, model, company):
      # Attributs d'instance
      self.model = model
      self.company = company
```

```python
c1 = Car() # va retourner une erreur
```

- Methodes

```python
def drive(self):
  print("La voiture roule")

def info(self):
  return f"Voiture: {self.model} - {self.company}"
```

- Héritage et Polymorphisme

```python
# voiture electric
class Tesla(Car):
    pass

# voiture automatic
class MBW(Car):
    pass
```

## Python VS Java en POO

Une petite comparaison entre Python et Java en POO

### Création de classe

- En Java

```java
public class Car {
    private String color;
    private String model;
    private int year;

    public Car(String color, String model, int year) {
        this.color = color;
        this.model = model;
        this.year = year;
    }

    public String getColor() {
        return color;
    }

    public String getModel() {
        return model;
    }

    public int getYear() {
        return year;
    }
}
```

- En Python

```python
class Car:
    def __init__(self, color, model, year):
        self.color = color
        self.model = model
        self.year = year
```

### Les attributs

- Java

```java
public class Car {
    private String color;
    private String model;
    private int year;
```

- Python

```python
def __init__(self, color, model, year):
    self.color = color
    self.model = model
    self.year = year
```

### Attributs ou variables de class

- Java

```java
public class Car {
    private String color;
    private String model;
    private int year;
    private static int wheels;

    public Car(String color, String model, int year) {
        this.color = color;
        this.model = model;
        this.year = year;
    }

    public static int getWheels() {
        return wheels;
    }

    public static void setWheels(int count) {
        wheels = count;
    }
}
```

- Python

```python
class Car:

    wheels = 0
```

### Public et Privé

- Java

```java
public class Car {
    String color; // public par default
    protected String model;
    private int year;
```

- Python

```python
class Car:

    wheels = 0

    def __init__(self, color, model, year):
        self.color = color # public
        self.model = model
        self.year = year
        self._cupholders = 6 # privé
```

### Accesseurs et Mutateurs

- Java

```java
public String getColor() {
    return color;
}

public void setColor(String color) {
    this.color = color;
}
```

- Python

Vous avez accès aux attributs directement

```python
my_car = Car("yellow", "beetle", 1969)
print(f"My car was built in {my_car.year}")


class Car:
    def __init__(self, color, model, year):
        self.color = color
        self.model = model
        self.year = year
        self._voltage = 12

    @property
    def voltage(self):
        return self._voltage

    @voltage.setter
    def voltage(self, volts):
        print("Warning: this can cause problems!")
        self._voltage = volts

    @voltage.deleter
    def voltage(self):
        print("Warning: the radio will stop working!")
        del self._voltage
```

### Self et This

- Java

```java
public void setColor(String color) {
    this.color = color;
}
// ou
public void setColor(String newColor) {
    color = newColor;
}
```

- Python

En python, le **self** est obligatoire

```python
class Car:
    def __init__(self, color, model, year):
        self.color = color
        self.model = model
        self.year = year
        self._voltage = 12

    @property
    def voltage(self):
        return self._voltage
```

### Méthode et Fonction

Python a des fonctions mais Java non.
Java a des méthodes, Python aussi.

- Java

```java
public class Main {
  static void myMethod() {
    // code to be executed
  }
}
```

- Python

```python
def my_function():
  print("Hi!")
```

Il reste des tonnes de choses à comparer.

Visitez [RealPython](https://realpython.com/oop-in-python-vs-java/) pour approfondire vos recherches.

## Me contacter

Twitter:[@xarala221](https://twitter.com/xarala221)
Linkedin:[Ousseynou DIOP](https://linkedin.com/in/xarala221)
Site Web: [www.xarala.co](https://www.xarala.co)
