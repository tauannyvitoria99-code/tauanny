# Simulador de Corrida de Carros (Threads em Java)

Trabalho II - POO II. Cada carro e uma Thread independente.

## Como executar
```
cd src
javac *.java
java Corrida
```

## Classes
- `Carro` (Runnable): avanca por passos aleatorios, dorme de 100 a 500 ms, faz pit stop na metade da prova e registra a chegada no podio.
- `Podio`: lista de classificacao protegida com `synchronized`.
- `Corrida`: cria os carros, guarda as Threads em `List<Thread>`, chama `start()` e `join()` e imprime o podio.
