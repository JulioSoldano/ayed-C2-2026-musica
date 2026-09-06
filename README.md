Clases del dominio (Pokemon, Receta, Cancion, Pokédex, LibroDeRecetas, Biblioteca, etc.).
# Lista global para almacenar las canciones
lista_canciones = []

def agregar_cancion(titulo, artista, album):
    cancion = {"titulo": titulo, "artista": artista, "album": album}
    lista_canciones.append(cancion)
    print(f"🎵 ¡'{titulo}' agregada con éxito!")

def mostrar_catalogo():
    if not lista_canciones:
        print("📭 El catálogo está vacío.")
        return
    print("\n--- CÁTALOGO DE CANCIONES ---")
    for i, c in enumerate(lista_canciones, 1):
        print(f"{i}. {c['titulo']} - {c['artista']} ({c['album']})")

Una clase por archivo. El CLI no debería conocer los detalles internos.
