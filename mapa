import matplotlib.pyplot as plt
import networkx as nx

# Crear un grafo dirigido
G = nx.DiGraph()

# Agregar nodos principales
G.add_node("Personas Morales")
G.add_node("1. Concepto")
G.add_node("2. Sociedades\nMercantiles")
G.add_node("3. Caracteristicas")
G.add_node("4. Obligaciones")
G.add_node("5. Formalizacion")

# Relacionar nodos principales
G.add_edge("Personas Morales", "1. Concepto")
G.add_edge("Personas Morales", "2. Sociedades\nMercantiles")
G.add_edge("Personas Morales", "3. Caracteristicas")
G.add_edge("Personas Morales", "4. Obligaciones")
G.add_edge("Personas Morales", "5. Formalizacion")

# Detallar el nodo "2. Sociedades Mercantiles"
sociedades = [
    "Sociedad Anonima (S.A.)", 
    "Sociedad de Responsabilidad\nLimitada (S. de R.L.)", 
    "Sociedad en Nombre Colectivo", 
    "Sociedad en Comandita", 
    "Sociedad Cooperativa"
]

for sociedad in sociedades:
    G.add_node(sociedad)
    G.add_edge("2. Sociedades\nMercantiles", sociedad)

# Detallar el nodo "3. Caracteristicas"
caracteristicas = [
    "Personalidad Juridica\nIndependiente", 
    "Patrimonio Propio", 
    "Finalidad Especifica", 
    "Duracion Indefinida o\nLimitada"
]

for caracteristica in caracteristicas:
    G.add_node(caracteristica)
    G.add_edge("3. Caracteristicas", caracteristica)

# Detallar el nodo "4. Obligaciones"
obligaciones = [
    "Registro en RFC", 
    "Pago de Impuestos (ISR, IVA)", 
    "Presentar Declaraciones", 
    "Llevar Contabilidad", 
    "Obligaciones Laborales"
]

for obligacion in obligaciones:
    G.add_node(obligacion)
    G.add_edge("4. Obligaciones", obligacion)

# Posicionar los nodos
pos = nx.spring_layout(G)

# Dibujar el grafo
plt.figure(figsize=(10, 8))
nx.draw(G, pos, with_labels=True, node_color='lightblue', node_size=3000, font_size=10, font_weight='bold', arrows=False)

# Mostrar el grafo
plt.title("Organizador Grafico de Personas Morales")
plt.show()
