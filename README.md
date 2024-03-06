# Algoritmo-de-Ordenação-insertion
def insertion_sort(arr):
    for i in range(1, len(arr)):
        key = arr[i]
        j = i - 1
        while j >= 0 and arr[j] > key:
            arr[j + 1] = arr[j]
            j -= 1
        arr[j + 1] = key

def main():
    tamanho_do_vetor = 30
    vetor = [2*i + 1 for i in range(tamanho_do_vetor)]  # Números ímpares
    print("Vetor original:")
    print(vetor)
    
    insertion_sort(vetor)
    
    print("\nVetor ordenado em ordem crescente:")
    print(vetor)

if _name_ == "_main_":
    main()
