
import random
import time

def rennen():
    print("Willkommen beim Rennspiel!")
    spieler1_position = 0
    spieler2_position = 0
    ziel = 50

    while spieler1_position < ziel and spieler2_position < ziel:
        input("Drücke Enter, um den nächsten Zug zu machen...")

        # Spieler 1 Zug
        spieler1_position += random.randint(1, 6)
        # Spieler 2 Zug
        spieler2_position += random.randint(1, 6)

        # Spielfeld anzeigen
        print("Spieler 1: " + "-" * spieler1_position + "🏎️")
        print("Spieler 2: " + "-" * spieler2_position + "🏎️")
        print("\n" + "-" * ziel)

        # Warten, um die Spannung zu erhöhen
        time.sleep(0.5)

    if spieler1_position >= ziel and spieler2_position >= ziel:
        print("Unentschieden!")
    elif spieler1_position >= ziel:
        print("Spieler 1 gewinnt!")
    else:
        print("Spieler 2 gewinnt!")

if __name__ == "__main__":
    rennen()
<!---
NautrioGX/NautrioGX is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
