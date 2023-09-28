def burbuja(lista):
  """
  Ordena una lista de números enteros usando el método de burbuja.

  Args:
    lista: La lista de números a ordenar.

  Returns:
    La lista ordenada.
  """

  n = len(lista)
  for i in range(n):
    for j in range(0, n - i - 1):
      if lista[j] > lista[j + 1]:
        lista[j], lista[j + 1] = lista[j + 1], lista[j]
  return lista

  
def seleccion(lista):
  """
  Ordena una lista de números enteros usando el método de selección.

  Args:
    lista: La lista de números a ordenar.

  Returns:
    La lista ordenada.
  """

  n = len(lista)
  for i in range(n - 1):
    min_pos = i
    for j in range(i + 1, n):
      if lista[j] < lista[min_pos]:
        min_pos = j
    lista[i], lista[min_pos] = lista[min_pos], lista[i]
  return lista


<!---
DalysCorrea15/DalysCorrea15 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
