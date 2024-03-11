import random

def player(prev_play, opponent_history=[]):
    # Check if it's the first game
    if prev_play == "":
        return random.choice(["R", "P", "S"])

    # Counter the opponent's last move
    if prev_play == "R":
        return "P"
    elif prev_play == "P":
        return "S"
    else:
        return "R"

# Uncomment the following lines if you want to test your player against another player (e.g., quincy)
# from RPS_game import play, quincy
# play(player, quincy, 1000, verbose=True)
