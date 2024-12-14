# Diferentes-Estruturas-Condicionais-ProZ-Educacao
Desenvolva um código que utiliza como seguintes características de um veículo: - Quantidade de rodas; - Peso bruto; - Quantidade de pessoas no veiculo. 
A: veiculo com duas ou três rodas; 
B: Veiculo com 4 rodas que acomodam até 8n pessoas e seu peso é de até 3500; 
C: Quatro rodas ou mais e com peso entre 3500 e 6000;
D: Veiculo com quatro rodas ou mais e que acomodam mais de 8 pessoas; 
E: Veiculo com quatro rodas ou mais e com mais de 6000 kg.

def categorize_vehicle(num_wheels, gross_weight_kg, num_passengers):
    """Categorizes a vehicle based on its characteristics.

  Args:
        num_wheels: O número de rodas do veículo.
        gross_weight_kg: O peso bruto do veículo em quilogramas.
        num_passengers: O número de passageiros que o veículo pode acomodar.

  Returns:
        Uma string representando a categoria do veículo (A, B, C, D ou E) ou "Desconhecido" se o veículo não se enquadrar em nenhuma categoria.
    """

  if num_wheels em (2, 3):
        retornar "A" # Duas ou três rodas
    elif num_wheels == 4 e num_passengers <= 8 e gross_weight_kg <= 3500:
        retornar "B" # Quatro rodas, até 8 passageiros, até 3500 kg
    elif num_wheels >= 4 e 3500 <gros_weight_kg <= 6000:
        retornar "C" # Quatro ou mais rodas, peso entre 3.500 e 6.000 kg
    elif num_wheels >= 4 e num_passengers > 8:
        retornar "D" # Quatro ou mais rodas, mais de 8 passageiros
    elif num_wheels >= 4 e peso_bruto_kg > 6000:
        retornar "E" # Quatro ou mais rodas, mais de 6.000 kg
    outro:
        return "Desconhecido" # Veículo não se enquadra em nenhuma categoria


# Exemplo de uso
veículo1 =categoria_veículo(2, 150, 2) # Motocicleta
veículo2 =categoria_veículo(4, 2000, 5) # Carro
veículo3 =categoria_veículo(6, 4500, 12) # Ônibus
veículo4 =categoria_veículo(4, 7000, 10) # Caminhão
veículo5 =categoria_veículo(3, 300, 1) # Triciclo

