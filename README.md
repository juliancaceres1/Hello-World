# Hello-World
# Definir una lista de diccionarios con los países y su PIB
paises_pib = [
    {"pais": "Estados Unidos", "pib": 21427000},
    {"pais": "China", "pib": 14723000},
    {"pais": "Japón", "pib": 5085000},
    {"pais": "Alemania", "pib": 4041000},
    {"pais": "Reino Unido", "pib": 2928000},
    {"pais": "India", "pib": 2875000},
    {"pais": "Francia", "pib": 2774000},
    {"pais": "Italia", "pib": 2092000},
    {"pais": "Brasil", "pib": 2023000},
    {"pais": "Canadá", "pib": 1751000}
]

# Ordenar la lista de países y su PIB en orden descendente
paises_pib_ordenados = sorted(paises_pib, key=lambda x: x["pib"], reverse=True)

# Generar una tabla con los países y sus capitales ordenados por PIB
tabla = "| País | PIB (en millones de dólares) |\n| --- | --- | --- |\n"
for pais_pib in paises_pib_ordenados:
    pais = pais_pib["pais"]
    pib = pais_pib["pib"]
    tabla += f"| {pais}  | {pib:,} |\n"

# Imprimir la tabla
print(tabla)
