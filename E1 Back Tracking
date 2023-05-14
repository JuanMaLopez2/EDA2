## E1. Dado un string, encontrar todas las permutaciones posibles que contengan todas las letras del string. Diseñe un algoritmo basado en fuerza bruta.

def generate_permutations(input_string, permutation, used_chars, permutations):
    if len(permutation) == len(input_string):
        permutations.append(permutation)
    else:
        for i in range(len(input_string)):
            if i not in used_chars:
                generate_permutations(input_string, permutation + input_string[i], used_chars | {i}, permutations)

def find_permutations(input_string):
    permutations = []
    generate_permutations(input_string, "", set(), permutations)
    for permutation in permutations:
        if set(input_string) == set(permutation):
            print(permutation)

input_string = ":'("
find_permutations(input_string)
