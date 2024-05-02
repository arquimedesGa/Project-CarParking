

# Car Parking System

This project implements a simple car parking system using the `Estacionamento` class.

## Usage

1. Create an instance of `Estacionamento` by providing initial price and price per hour.
2. Add vehicles using the `AdicionarVeiculo()` method.
3. Remove vehicles using the `RemoverVeiculo()` method.

## Example

```csharp
using System;

namespace Project_CarParking.models
{
    class Program
    {
        static void Main(string[] args)
        {
            // Initialize parking system
            Estacionamento parking = new Estacionamento(precoInicial: 5, precoPorHora: 2);

            // Add a vehicle
            parking.AdicionarVeiculo();

            // Remove a vehicle
            parking.RemoverVeiculo();

            // Display total price
            Console.WriteLine($"Total price: {parking.ValorTotal}");
        }
    }
}
