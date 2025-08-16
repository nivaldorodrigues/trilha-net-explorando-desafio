# DIO - Trilha .NET - Explorando a linguagem C#
www.dio.me

## Desafio de projeto
Para este desafio, você precisará usar seus conhecimentos adquiridos no módulo de explorando a linguagem C#, da trilha .NET da DIO.

## Contexto
Você foi contratado para construir um sistema de hospedagem, que será usado para realizar uma reserva em um hotel. Você precisará usar a classe Pessoa, que representa o hóspede, a classe Suíte, e a classe Reserva, que fará um relacionamento entre ambos.

O seu programa deverá cálcular corretamente os valores dos métodos da classe Reserva, que precisará trazer a quantidade de hóspedes e o valor da diária, concedendo um desconto de 10% para caso a reserva seja para um período maior que 10 dias.

## Regras e validações
1. Não deve ser possível realizar uma reserva de uma suíte com capacidade menor do que a quantidade de hóspedes. Exemplo: Se é uma suíte capaz de hospedar 2 pessoas, então ao passar 3 hóspedes deverá retornar uma exception.
2. O método ObterQuantidadeHospedes da classe Reserva deverá retornar a quantidade total de hóspedes, enquanto que o método CalcularValorDiaria deverá retornar o valor da diária (Dias reservados x valor da diária).
3. Caso seja feita uma reserva igual ou maior que 10 dias, deverá ser concedido um desconto de 10% no valor da diária.

![Diagrama de classe estacionamento](diagrama_classe_hotel.png)

## Solução
O código está pela metade, e você deverá dar continuidade obedecendo as regras descritas acima, para que no final, tenhamos um programa funcional. Procure pela palavra comentada "TODO" no código, em seguida, implemente conforme as regras acima.

---

## O que já foi implementado

- **Validação da capacidade da suíte:** O método `CadastrarHospedes` verifica se a quantidade de hóspedes não excede a capacidade da suíte, lançando uma exceção caso contrário.
- **Cadastro da suíte:** O método `CadastrarSuite` permite associar uma suíte à reserva.
- **Quantidade de hóspedes:** O método `ObterQuantidadeHospedes` retorna corretamente o número de hóspedes cadastrados.
- **Cálculo do valor da diária:** O método `CalcularValorDiaria` calcula o valor total da reserva multiplicando os dias reservados pelo valor da diária da suíte e aplica um desconto de 10% automaticamente para reservas de 10 dias ou mais.

Essas implementações garantem que as principais regras de negócio do desafio sejam atendidas, tornando o sistema funcional até o ponto de permitir o cadastro de hóspedes e suítes, bem como o cálculo do valor da diária com desconto apropriado.
