def main():
    import time
    print(f"Hi! Welcome to UnityGrid Access!")
    print(f"What game would you like to access?")
    gc = input("1 : Tic Tac Toe , 2 : EnigmaDigits , 3 : Guardians of the Meridiaan , 4 : Exit : ")
    if gc == '1':
        
        tictactoe()
        time.sleep(2)
        print("1 : Return to Main Menu")
        time.sleep(1)
        print("2 : Replay")
        time.sleep(1)
        print("3 : Leave Game")
        time.sleep(1)
        wwy = str(input(": "))
        if wwy == '1':
            main()
        elif wwy == '2':
            tictactoe()
        else:
            sys.exit(0)
        
    elif gc == '2':

        enigmadigits()
        time.sleep(2)
        print("1 : Return to Main Menu")
        time.sleep(1)
        print("2 : Replay")
        time.sleep(1)
        print("3 : Leave Game")
        time.sleep(1)
        wwy = str(input(": "))
        if wwy == '1':
            main()
        elif wwy == '2':
            enigmadigits()
        else:
            sys.exit(0)

    elif gc == '3':
        GOM() 
        
        

    else:
        sys.exit(0)

def egr():
    if status == ended:
        print("What would you like to do?")
        print("1 : Return to Main Menu")
        print("2 : Replay")
        print("3 : Leave Game")
        wwy = str(input(": "))
        if wwy == '1':
            main()
        elif wwy == '2':
            if gid == 1:
                tictactoe()
            elif gid == 2:
                enigmadigits()
            else:
                GOM()
        else:
            sys.exit(0)
def tictactoe():
    import random
    import time
    gid = str('1')
    class TicTacToe:

        def __init__(self):
            self.board = []

        def create_board(self):
            for i in range(3):
                row = []
                for j in range(3):
                    row.append('-')
                self.board.append(row)

        def get_random_first_player(self):
            return random.randint(0, 1)

        def fix_spot(self, row, col, player):
            self.board[row][col] = player

        def is_player_win(self, player):
            win = None

            n = len(self.board)

            # checking rows
            for i in range(n):
                win = True
                for j in range(n):
                    if self.board[i][j] != player:
                        win = False
                        break
                if win:
                    return win

            # checking columns
            for i in range(n):
                win = True
                for j in range(n):
                    if self.board[j][i] != player:
                        win = False
                        break
                if win:
                    return win

            # checking diagonals
            win = True
            for i in range(n):
                if self.board[i][i] != player:
                    win = False
                    break
            if win:
                return win

            win = True
            for i in range(n):
                if self.board[i][n - 1 - i] != player:
                    win = False
                    break
            if win:
                return win
            return False

            for row in self.board:
                for item in row:
                    if item == '-':
                        return False
            return True

        def is_board_filled(self):
            for row in self.board:
                for item in row:
                    if item == '-':
                        return False
            return True

        def swap_player_turn(self, player):
            return 'X' if player == 'O' else 'O'

        def show_board(self):
            for row in self.board:
                for item in row:
                    print(item, end=" ")
                print()

        def start(self):
            self.create_board()

            print("Loading...Please Wait")
            time.sleep(3)
            print(r"""


                 _____ _        _____            _____          
                |_   _(_) ___  |_   _|_ _  ___  |_   _|__   ___ 
                  | | | |/ __|   | |/ _` |/ __|   | |/ _ \ / _ \
                  | | | | (__    | | (_| | (__    | | (_) |  __/
                  |_| |_|\___|   |_|\__,_|\___|   |_|\___/ \___|
                      


                      """)
            time.sleep(1)
            player = 'X' if self.get_random_first_player() == 1 else 'O'
            while True:
                

                print(f"Player {player} turn")

                self.show_board()

                # taking user input
                row, col = list(
                    map(int, input("Enter row and column numbers to fix spot: ").split()))
                print()

                # fixing the spot
                self.fix_spot(row - 1, col - 1, player)

                # checking whether current player is won or not
                if self.is_player_win(player):
                    print(f"Player {player} wins the game!")
                    break

                # checking whether the game is draw or not
                if self.is_board_filled():
                    print("Match Draw!")
                    break

                # swapping the turn
                player = self.swap_player_turn(player)

            # showing the final view of board
            print()
            self.show_board()


    # starting the game
    tic_tac_toe = TicTacToe()
    tic_tac_toe.start()
    

def GOM():
            print(r"""
                  ____                     _ _                          __   _   _          
                 / ___|_   _  __ _ _ __ __| (_) __ _ _ __  ___    ___  / _| | |_| |__   ___ 
                | |  _| | | |/ _` | '__/ _` | |/ _` | '_ \/ __|  / _ \| |_  | __| '_ \ / _ \
                | |_| | |_| | (_| | | | (_| | | (_| | | | \__ \ | (_) |  _| | |_| | | |  __/
                 \____|\__,_|\__,_|_|  \__,_|_|\__,_|_| |_|___/  \___/|_|    \__|_| |_|\___|
                                 __  __           _     _ _                                                 
                                |  \/  | ___ _ __(_) __| (_) __ _  __ _ _ __                                
                                | |\/| |/ _ \ '__| |/ _` | |/ _` |/ _` | '_ \                               
                                | |  | |  __/ |  | | (_| | | (_| | (_| | | | |                              
                                |_|  |_|\___|_|  |_|\__,_|_|\__,_|\__,_|_| |_|                               """)
            print()
            print()
            print("Loading...Please wait")
            print("")
            print("")
            print("")
            time.sleep(3)
            print("""


                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⠎⡜⢠⣾⡿⣫⡄⢀⡔⠁⠀⠀⢠⡾⣷⣿⣿⣿⣿⡄⠘⢷⣵⡌⢳⣎⠻⣧⣱⡜⣆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡌⡘⣰⢛⣿⣿⣿⣷⡿⠊⠀⠀⢠⢎⣴⡿⠛⠉⠹⣿⣷⣄⠈⢻⣞⣎⢿⣷⣌⢿⢿⣾⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⣱⡿⠃⣸⣟⣽⣿⣟⣡⡔⠀⡰⢡⣾⡞⡇⠀⠀⠀⣿⣿⣯⣟⢆⢻⣿⣿⣿⡼⣮⡙⣿⡼⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣤⠞⢡⠃⣰⣿⣿⣿⣿⡿⠻⣴⣾⣷⣿⠋⣰⠀⠀⠀⠀⢿⣿⣿⣿⣎⢫⣿⣿⣿⣿⣿⣷⣼⣷⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⠟⢁⡰⢋⣼⣿⣿⣿⣯⣴⣯⣿⣿⣿⣿⠃⣠⠃⠀⠀⠀⠀⠘⣿⣿⣿⣿⣧⠹⣿⣿⣿⣿⢿⣿⣿⣿⡶⠤⠤⠤⠖⠁⠀⠀⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⢋⣴⣿⣧⣾⣿⣿⣟⣷⣷⣹⣿⣿⠏⢹⢏⠝⠛⠶⣤⣀⡀⠀⠀⠸⣿⣿⣿⡻⣧⡹⣿⣿⡝⣿⣿⣿⣿⣷⣀⡀⠀⠀⠀⢀⡤⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣯⣿⣇⣿⣿⣿⣿⣿⡇⠻⢩⣟⣻⡿⣸⣿⢿⣿⣷⣶⣶⣿⣿⡶⠄⠀⠹⡝⣿⣜⣮⣷⣿⣿⣿⣿⡿⢿⣿⣿⣿⡿⣷⣦⣴⣿⠵⠃⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⡏⢱⣿⣿⡿⢻⣿⣿⣿⣼⣱⣼⣿⣿⢿⡏⠈⠻⢿⣟⡃⠻⠟⠀⠀⠀⣠⣾⣿⣿⣶⣶⣼⣿⣿⣿⣿⣾⣿⣿⣿⣿⣿⣿⠉⠁⠀⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⡇⡞⡟⠋⣠⣾⣿⣿⣿⣿⣭⣿⣿⠋⠈⢷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠰⠋⠛⢿⣯⡼⢿⣿⣿⣿⣿⣿⣿⣿⣿⢿⣿⣿⣿⣦⣀⠄⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢷⠁⣧⣾⣿⣿⣿⣿⣿⣿⣿⣿⣿⡄⠀⠸⡃⠀⠀⠀⠀⠀⠀⠀⠀⣶⠀⠀⠀⠀⢠⣿⣿⣿⣿⣿⣿⣽⣿⣿⣻⢿⠎⠿⡗⠙⡄⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢷⣿⣿⣏⠻⣿⣿⣯⠿⣿⣿⣿⣷⠀⠀⠑⠀⠀⠀⠀⠀⠠⠤⣠⡾⠃⠀⠀⢀⣾⣿⣿⣿⣿⣿⣿⣿⣿⡿⣿⣿⠀⣠⡇⠴⠃⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⣌⣻⣦⣟⣿⣿⣿⣿⣿⣿⣟⣧⡀⠀⠀⠀⣀⣀⣀⣀⣀⡉⠀⠀⠀⢠⣾⣿⣿⣿⣿⣿⣿⣿⡿⣿⣿⢸⣿⢀⠞⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⠧⠼⢧⡖⢺⢻⣿⣿⣿⡇⠹⣷⣄⠀⠀⠀⠉⢿⣽⣿⠓⠂⢀⣴⣿⣿⣿⣿⣿⣿⣿⣿⣿⠁⢈⣿⡿⠏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢃⠀⠉⠓⠊⢸⡿⡿⠇⠀⠙⣿⣷⣄⠀⠀⠀⠀⠀⢀⣴⣿⣿⣿⣿⠛⣿⣿⡿⢟⣿⣃⠴⠛⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⣾⣯⣶⡤⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣸⠀⠀⠀⠀⠀⠘⣿⣿⣷⣦⣤⣤⣶⡋⢿⡉⠛⢛⡓⢊⣼⡿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⢙⣿⣿⣷⣿⣭⡶⣤⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⡇⠀⠀⠀⠀⠀⠀⠈⢿⣿⣿⣿⡟⠼⠓⠦⠙⠂⠉⠒⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⣿⣿⣱⣿⡿⣻⣶⣯⣼⣿⠲⢄⡀⠀⠀⠀⠀⡠⠲⣶⣦⡞⠀⠀⠀⠀⠀⠀⠀⠀⣜⣿⣿⣿⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⠛⠿⣿⣿⣿⣿⣿⣻⣿⢿⣷⣿⣼⣗⣦⣀⠞⣠⣾⣿⣿⠃⠀⠀⠀⠀⠀⠀⠀⠀⢹⣿⣿⣾⣎⢷⣤⡀⠀⠀⣀⢠⠤⢤⠒⠶⠖⠒⠲⢶⣄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⠀⠀⠈⠙⠻⣿⣿⣿⣿⣼⣿⠟⣿⣿⣿⢫⣶⣿⣿⣿⣏⣵⠦⠠⣤⣄⡀⠀⠀⠀⠈⣿⣿⣿⣿⡆⠳⡻⣟⠻⢧⣄⣽⣲⣄⠀⠀⠀⠀⣴⣌⠛⠒⢦⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠉⠻⢿⣿⣿⣿⣿⣩⣷⣿⣿⣿⠿⠛⣫⡤⠂⢠⣬⣷⣌⠉⠒⠒⠷⣽⣿⣿⡿⣿⡀⠁⠈⢧⣄⡈⠙⢟⣿⣧⡀⠀⠀⣿⢻⣦⢀⣆⡭⠓⠒⠲⡄⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢙⡿⣿⣿⣿⣿⡏⢀⡴⠚⣡⡴⠃⢀⣀⠀⠉⠳⢤⡀⠀⠈⠻⣧⣤⣿⣷⠈⠆⠘⢫⡿⣦⡀⠙⢄⢻⣷⣄⣿⠀⣨⣿⠃⠀⣀⡴⣢⣇⣀⡀⠀⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⠀⢀⣴⠾⠛⠉⣿⣿⣿⣿⣽⣧⣤⡟⢁⣴⠶⠋⣀⣶⣄⡀⠀⠉⠓⠦⣀⠈⠙⠇⢻⣇⠀⠀⠈⣿⡿⣷⡄⠈⢎⣿⣿⣿⢠⣿⣿⣠⣾⠏⡠⠟⠛⠁⠸⣆⠀⠀⠀
                ⠀⠀⠀⠀⠀⠀⢀⡏⠁⠀⠀⠸⣿⣿⣿⣿⠿⣿⣿⣷⣸⣷⢲⣾⣿⣿⣿⣿⣆⠀⠀⠀⠈⠙⠶⣄⡀⢿⡄⠀⠀⢸⣿⡞⣿⣆⠸⣽⣿⣿⣾⣿⣿⡿⣵⡏⠀⢀⡴⠊⠀⢹⣷⣤⣀
                ⠀⠀⠀⠀⠀⠀⣾⠀⠀⠀⠤⣀⣿⣿⣿⠋⠈⠛⠿⡿⣿⣿⣼⣿⣻⣿⣿⣿⣿⣷⣄⠀⠀⠀⠀⠀⠙⠺⢧⡀⠀⠀⢫⢷⣸⣿⢧⢹⣿⣿⣿⣿⣿⠟⣿⢁⠔⠋⣠⣶⣾⣯⣤⠟⣿
                ⠀⠀⠀⠀⠀⣸⡿⠀⠀⠀⠀⠙⢮⡻⣿⣷⡄⠀⡇⠀⠀⢿⣿⣿⣿⣷⣼⣿⢿⣿⣿⣿⣦⣀⠀⣠⡤⠀⠀⠈⠑⠢⣼⣼⣿⡿⣾⣏⠿⣿⣿⣿⣧⣿⣿⣥⣾⣿⡿⣛⣿⡿⠞⠋⠀
                ⠀⠀⠀⠀⢰⣿⠀⠀⠀⠀⠀⠀⠀⣈⣎⢿⡿⡀⢹⣠⢧⠆⠙⠻⢿⠿⣿⣿⣿⣿⣿⣿⣿⣾⣟⣿⣷⣶⣄⠀⠀⠀⠀⠙⠻⣷⡸⣿⡄⢹⣿⣿⣿⣿⣿⣿⣿⣷⣯⣵⠶⠀⠀⠀⠀
                ⠀⠀⠀⠀⣸⢻⡄⠀⠀⠀⠀⠀⠳⣽⣞⣆⠻⣷⣼⣿⠿⠀⠀⠀⠀⠀⠈⠙⠿⣿⣿⣿⣿⣿⣿⣷⣽⣿⣿⣷⣄⠀⠀⠀⠀⠀⠙⠻⢯⣀⣻⣿⣿⣿⣿⣻⡿⠟⠉⠀⠀⠀⠀⠀⠀
                ⠀⠀⠀⣼⣡⣶⣿⣦⡀⠀⠀⠀⢶⡾⣿⣿⣧⢹⣷⣿⡇⠀⡀⡄⠀⠀⠀⠀⠀⠉⠻⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣄⡀⠀⠀⠀⠀⠀⢹⣿⣻⠿⣿⠿⠿⠮⢅⣛⣿⣿⡿⢿⣿⣿
                ⠀⠀⠀⠹⣿⣿⣿⡿⡻⣆⡀⠀⠈⣆⢿⣿⣿⣧⣻⣿⡇⣸⢻⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⢿⣿⣿⣿⣿⣿⣿⣷⣿⡻⣿⣷⣄⠀⠀⠀⢸⣽⣮⠀⠹⣟⢷⣶⣤⣤⣤⣥⣀⣀⡀⠉
                ⠀⠀⠀⠀⢹⣮⣿⣟⢄⠀⠙⢿⣶⣾⣎⣿⣿⣿⣿⣿⣧⢿⣷⣿⢧⠂⠀⡴⠀⠀⠀⠀⠀⠀⠙⢿⣿⣿⣿⣿⣿⣿⣿⣾⠿⠛⢳⣤⡀⠀⢿⣿⣆⠀⣿⣦⠈⠉⠛⠻⢿⣿⣿⣿⣿
                ⠀⠀⠀⣰⣿⣿⣿⣾⣦⣀⠀⠀⠝⣻⣿⣿⣿⣿⣿⣿⣿⣿⣿⢧⠇⢀⠞⠁⠀⠀⠀⠀⠀⠀⠀⠀⣻⡟⠻⣿⣿⠟⠁⣀⣤⣶⣿⣿⣿⣦⣌⢿⣻⡐⣿⣿⣷⣤⣤⣤⣀⡈⠙⠻⢿
                ⠀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣷⣦⡺⣿⣷⡻⣿⣿⣿⣿⣿⣿⣯⣮⣎⣥⠴⠒⠀⠀⠀⠀⠀⠀⠀⢠⣿⡇⢀⡼⠁⣰⣿⣿⣿⡿⠿⢿⣿⣿⣿⣿⣿⣷⡹⣿⣿⣝⢿⣿⣿⣿⣿⣦⣄
                ⠀⠀⠀⢻⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣮⡻⣿⣿⣿⣏⣾⣿⣿⣿⣶⣤⡀⠀⠀⠀⠀⠀⠀⣾⣿⣧⠞⢁⣴⠿⠟⠋⢁⣠⣖⣀⡉⠻⣿⣿⣿⣿⣷⡝⣿⣿⣧⠻⣿⣿⣿⣿⣿


                """)
            print(f"Hello traveler, I am the goddess of of reincarnation Aionia")
            time.sleep(2)
            print("Through my mistake I have unfortunatly caused your untimely demise...")
            time.sleep(3)
            print("As compensation for my mistake, I will reincarnate you in another world filled with magic and swordmanship.")
            print("I will give you 2 skill sets to choose from before you start your journey...")
            time.sleep(3)
            print(r"""1 : Celestior the Starweaver : Skills include : Receptive Language, Celestine Scepter, Cerebral Surge, Incantation Imperium, Mana Flux,
                  and the Special Ability : Rain of Annihilation""")
            time.sleep(1)
            print(r"""2 : Bladebound Sentinel : Skills include : Receptive Language, Sword of Annihilation, Agility, Enhanced Strength and Endurance,
                  and the Special Ability : Slash of Annihilation""")
            global choice_skill
            choice_skill = input("What skill set do you want? : ")
            
            
            time.sleep(2)
            print("...")
            time.sleep(2)
            print(f"As you wish traveler, Good Luck...")
            time.sleep(2)
            print("No offence but, try not to die, I don't want to see you here any time soon (─▽─) ")
            time.sleep(3)
            print(r"""








































                    
                    """)
            time.sleep(3)
            print(r"""










                                                                           |>>>
                                   _                      _                |
                    ____________ .' '.    _____/----/-\ .' './========\   / \
                   //// ////// /V_.-._\  |.-.-.|===| _ |-----| u    u |  /___\
                  // /// // ///==\ u |.  || | ||===||||| |T| |   ||   | .| u |_ _ _ _ _ _
                 ///////-\////====\==|:::::::::::::::::::::::::::::::::::|u u| U U U U U
                 |----/\u |--|++++|..|'''''''''''::::::::::::::''''''''''|+++|+-+-+-+-+-+
                 |u u|u | |u ||||||..|              '::::::::'           |===|>=== _ _ ==
                 |===|  |u|==|++++|==|              .::::::::.           | T |....| V |..
                 |u u|u | |u ||HH||         \|/    .::::::::::.
                 |===|_.|u|_.|+HH+|_              .::::::::::::.              _
                                __(_)___         .::::::::::::::.         ___(_)__
                ---------------/  / \  /|       .:::::;;;:::;;:::.       |\  / \  \-------
                ______________/_______/ |      .::::::;;:::::;;:::.      | \_______\________
                |       |     [===  =] /|     .:::::;;;::::::;;;:::.     |\ [==  = ]   |
                |_______|_____[ = == ]/ |    .:::::;;;:::::::;;;::::.    | \[ ===  ]___|____
                     |       |[  === ] /|   .:::::;;;::::::::;;;:::::.   |\ [=  ===] |
                _____|_______|[== = =]/ |  .:::::;;;::::::::::;;;:::::.  | \[ ==  =]_|______
                 |       |    [ == = ] /| .::::::;;:::::::::::;;;::::::. |\ [== == ]      |
                _|_______|____[=  == ]/ |.::::::;;:::::::::::::;;;::::::.| \[  === ]______|_
                   |       |  [ === =] /.::::::;;::::::::::::::;;;:::::::.\ [===  =]   |
                ___|_______|__[ == ==]/.::::::;;;:::::::::::::::;;;:::::::.\[=  == ]___|_____










                """)
            print("A Village, Nice of god to drop me off here.")
            time.sleep(1)
            print("*turns around*")
            time.sleep(1)
            print(r"""










                        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⠧⠒⠉⠁⠀⢀⠀⠀⠀⠀⣀⠔⠓⠂⠐⠊⢉⠤⢄⠠⠤⣈⡁⠒⠒⠚⠷⠖⠈⠉⡩⠥⡀⠉⠋⡗⢄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⠞⠉⠀⠀⠀⠀⡠⠊⢃⠀⠐⠋⢀⡀⠀⠀⢠⠔⠊⠀⠀⠀⠀⠀⠑⢄⠀⠀⠃⠀⠀⠞⠀⠀⠑⢄⠀⠃⠀⠀⠘⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣸⠝⠂⠀⠀⠀⡠⠊⠁⠀⠈⡄⠀⠀⡇⠀⠑⠀⢸⠄⠀⠀⠀⠀⡠⠤⢀⠈⡀⠀⠲⠀⢰⠀⠀⠀⠀⠈⡧⢀⠀⠀⠀⢡⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⠖⠃⠀⠀⠀⠀⡐⠁⠀⠀⠀⠀⠠⠠⠊⠀⣀⣀⠄⠊⠀⠀⠀⠀⡜⠀⠀⠀⠑⢼⡀⠀⠀⡌⠀⠀⠀⠀⠀⢨⢄⠈⢢⣄⠀⠑⢄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣤⠞⠁⠀⠀⡠⠊⠉⢈⠠⠴⠊⢢⠀⠀⡼⠀⠀⠀⠀⠀⠀⠀⠀⠠⠋⠈⠁⠀⠀⠀⢀⠘⡈⢢⠜⠀⠀⠀⠀⠀⠀⠀⠑⠠⠈⠢⠑⠄⡀⠀⠁⠒⠠⢄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⠃⠀⠀⢀⠎⠀⡰⠒⠁⠀⠀⠀⢠⠂⠀⠑⠐⠒⠀⠐⢄⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⠎⠑⢲⡀⠀⠀⠀⠀⠀⣠⠤⡀⠀⠀⠀⠀⠀⣀⣈⠡⠈⠦⣤⡀⠡⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣠⣖⠯⠐⠀⠀⠀⠀⢠⠃⠀⠀⠀⠀⠀⠘⠆⠀⠀⠀⠀⠀⠀⠈⠃⠀⢀⡠⠐⠂⠘⠀⢀⠎⠀⠀⠀⠀⠉⠅⠐⠢⡀⠀⠀⠈⠂⠒⠂⠠⠤⡀⠀⠓⡄⠀⠀⣘⡂⣣⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡔⡏⠄⠀⠀⠀⠀⠀⢀⣂⠁⠀⠀⠀⠀⠀⢀⡀⠘⠂⠀⠐⠒⠢⢀⠀⠀⠈⠉⡤⢀⡀⠀⠀⠋⠀⠀⣀⣀⠀⠀⠀⠀⠀⠈⠒⠀⠀⠀⠀⠀⠀⠀⠈⠂⠴⠀⠀⠀⠀⠀⠀⠡⠑⠦⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢧⡡⠐⢄⠢⠤⡤⠒⠪⠉⠐⢄⠀⠀⢀⡠⡎⡑⠠⠀⡠⠂⠀⠠⢈⣦⡄⡀⠀⢱⠈⠁⠂⠀⠀⠤⠔⡉⠉⠂⠀⠀⠀⢀⠀⠀⠀⡀⠤⠠⠤⢀⠀⠀⠀⠀⠀⢀⣀⠠⡤⡴⡖⠒⠂⣹⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠒⠛⠳⠶⠥⠖⢬⢲⣦⠵⢤⡨⢆⣈⣁⣀⢡⡐⣄⢣⡐⡄⠀⢢⡀⠸⢿⣴⣕⣂⡀⠀⡇⠀⠀⠀⠀⣇⠤⢒⣓⣀⡤⠄⡷⠶⢡⡤⣤⡶⡶⢬⡿⢿⠭⢝⣿⣛⣷⣾⣿⡕⢴⠥⠒⠉⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠑⠺⠦⢤⣌⢒⠠⠄⡘⣭⣍⠻⣛⣳⣾⣅⣀⡈⠽⣧⣼⠢⣙⣿⣮⠂⢄⡀⠀⢠⣷⣜⠫⣟⣗⠠⡾⠊⣀⣠⠿⠴⠿⡻⠉⣰⣥⣔⣥⠶⠛⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⠉⠐⠺⢍⣛⣛⣟⣿⣿⣿⣦⠹⠷⢶⡈⡛⠺⣾⡿⣿⠒⣛⣿⠭⣿⡿⢻⣏⣠⡾⠟⡳⠏⠕⢉⣰⣮⣴⠞⠛⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠋⠷⢤⢹⢳⢳⢿⡝⡟⠥⠜⡟⢡⣾⡻⣶⢿⣯⠶⠿⠛⠛⠉⠉⠉⠉⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠹⣟⠂⡎⣯⠸⣸⢱⣇⢬⣼⣷⡏⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⣷⠉⠃⡇⢾⡈⢸⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⢏⡌⣰⣿⣿⠧⡸⣎⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣸⣿⣏⣼⣿⣠⡙⡟⢿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⠏⡾⢹⢿⣇⢋⣾⢱⣜⣿⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣴⣯⡟⣽⡿⣜⢮⣉⠚⡁⣨⣯⣿⡻⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣠⣾⣿⠏⣱⠟⣴⣯⣄⣩⣙⣻⣬⣘⣌⠿⡿⢷⢤⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡀⢀⢤⠀⠀⢀⣼⣫⣵⣯⣇⣰⣯⣾⣿⣿⣴⣴⣛⣾⣿⣬⣛⡛⠾⡳⢷⣍⣛⠶⣤⣀⣀⣀⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣰⣶⣷⠶⢿⡿⠾⠟⣫⠿⣟⣩⠿⡽⠛⢹⣿⣿⣿⣿⡜⠺⢀⠝⢻⣄⠻⢿⣷⠿⣿⣯⣙⡟⣾⣿⣿⡟⠛⠿⡿⠿⠟⠛⠶⡛⣳⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣤⣔⣻⡿⣿⣿⣿⣿⣷⣾⣚⣀⣤⠾⢿⡞⢋⠼⠞⢀⣴⣿⢿⣿⣿⣆⡣⠙⠬⠒⢬⣜⣧⣢⣙⣷⢿⣿⣿⣿⡿⠿⠿⣿⢿⣯⣭⣁⣶⣖⣒⣺⣖⠛⠛⢾⣿⣶⣶⣶⣶⣶⣶⣶⣶⣦⣄⣀⣀⣀⠀⠀⠀⠀⠀⠀
                        ⠠⠤⠤⠴⠶⣶⠶⣾⣶⣶⣶⣶⣶⡾⠿⢿⣿⣿⣿⣿⣯⣤⣾⠿⠿⣿⣿⣷⣿⣷⣾⣷⡶⠾⣛⣻⣿⣿⣿⣿⣶⣿⣭⣿⣿⣶⣷⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣻⣟⣟⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡿⠷⠤⠬⠭⠥⠤⠤⠤⠄
                        ⠀⠀⠀⠀⠐⠛⠒⠉⠩⠽⣿⣿⣯⣥⣤⣬⣿⣿⣿⣿⣙⡛⠋⠀⠀⠉⠉⠉⠍⠩⠉⠩⠥⠤⠩⠭⠩⠯⠉⠉⠉⠉⠉⠉⠉⠉⠉⠉⠉⠩⣉⣉⣉⣉⣉⣉⣉⡉⠉⠉⠉⠉⠩⠭⠭⠉⠛⠋⠋⠛⠙⠋⠉⠉⠉⠉⠉⠉⠉⠉⠉⠉⠉⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀
                        ⠀⠀⠀⠀⠉⠁⠈⠁⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀










                """)
            time.sleep(1)
            print("Wow...That must be Yggdrasil...apparently only I can see it")
            time.sleep(1)
            print("Well for now I'm just going to go to the Village")
            time.sleep(1)
            print("Guard : Looking to enter the village?")
            time.sleep(1)
            print("Yea")
            time.sleep(1)
            print("Guard : Wheres your Identification?")
            time.sleep(1)
            print("I don't have any Identification")
            time.sleep(1)
            print("Guard : Oh, ok then just put your hand over this orb.")
            time.sleep(1)
            print("Why?")
            time.sleep(1)
            print("Guard : The orb will determine your intentions, and based on that we will determine if you are able to enter the village")
            time.sleep(1)
            print("Ok")
            time.sleep(1)
            print("*hovers hand over the orb*")
            time.sleep(1)
            print("*orb glows blue*")
            time.sleep(1)
            print("Guard : Ah, a blue glow you must have a pure heart. Welcome to the village of Sundawn Hollow traveler")
            time.sleep(1)
            print("Thank you")
            time.sleep(1)
            print("Guard : You should probably go make an identification card at the adventurers guild")
            time.sleep(1)
            print("Ok, thank you for the information")
            time.sleep(1)
            print("*Entering Village...*")
            time.sleep(1)
            print("Loading...Please wait")
            time.sleep(2)
            while True:
                print("Where should  I go...")
                time.sleep(1)
                print("1 : Adventurers Guild")
                time.sleep(1)
                print("2 : Stroll around the village")
                xs = input(": ")
                if xs == '1':
                    gag()
                    break
                elif xs == '2':
                    stv()
                    break
                else:
                    print("\nInvalid Input Please input a valid value")

            
            
                    
                    
def gag():
    print("*Entering Adventurers Guild*")
    print("Loading...Please Wait")
    time.sleep(2)
    print("Receptionist : Welcome to the Pathfinder’s Pantheon Guild")
    time.sleep(1)
    print("Receptionist : How may I help you")
    time.sleep(1)
    print("I'm here to make an Identification card")
    time.sleep(1)
    print("Receptionist : Ok, Please wait a moment")
    time.sleep(1)
    print("Receptionist : Please fill out this form")
    an = str(input("Name : "))
    ap = str(input("Profession : "))
    aa = str(input("Age : "))
    an1 = an.capitalize()
    ap1 = ap.capitalize()
    aa1 = aa.capitalize()
    time.sleep(1)
    print("Receptionist : Alright, Please wait a moment while we make your card")
    time.sleep(1)
    print("*1 hour later*")
    time.sleep(2)
    print(f"""Receptionist : Alright {an1} here is your card, try not to lose it, it has all your information on it
            and remaking the card is going to make a while""")
    time.sleep(1)
    print("Thank you")
    time.sleep(1)
    print("Receptionist : You should be careful whey you go take on a quest")
    time.sleep(1)
    print("Why?")
    time.sleep(1)
    print("Receptionist : It was said NECRON will awaken this year...")
    time.sleep(1)
    print("1 : Who's NECRON")
    time.sleep(0.5)
    print("2 : Ok, Thank you for the information")
    nqw(an1, ap1, aa1)
def nqw(an1, ap1, aa1):
    nc = input(": ")
    if nc == '1':
        necronq(an1)
    elif nc == '2':
        tyfti(an1, ap1, aa1)
    else:
        print("Please input a valid input")
        nqw(an1, ap1, aa1)
                
def tyfti(an1, ap1, aa1):
    import time
    time.sleep(1)
    print("""










        """)
    print("What should I do next?")
    time.sleep(1)
    print("1 : Go to Inn")
    print("2 : Pick Quest")
    agc = input(": ")
    if agc == '1':
        gti(an1, aa1, ap1)
    else:
        pq(an1, choice_skill)

def pq(an1, choice_skill):
    import time
    time.sleep(1)
    print("Hey I want to start a quest.")
    time.sleep(1)
    print(f"Receptionist : Oh! {an1} I have 2 quests available at the moment.")
    time.sleep(1)
    print("1 : Mountain Bear Subjugation Quest")
    print("2 : Demon Wolf Subjugation Quest")
    cq = input(": ")
    if cq == '1':
        print(f"Alright, {an1} the reward of this quest is 70 Silver")
        time.sleep(1)
        print("The bear was spotted in the mountains south of the village")
        time.sleep(1)
        print("Alright I'll head there and Subjugate the bear.")
        time.sleep(1)
        print("*Traveling to the Mountains*")
        time.sleep(1)
        print("Loading...Please wait")
        time.sleep(3)
        print("You see the bear destroying trees as you arive to the site.")
        time.sleep(1)
        print("Thats a big Bear")
        time.sleep(1)
        print("What skill should I use")
        time.sleep(1)
        print("1 : Stabbing Barrage")
        print("2 : Slash of Destruction")
        cqm = input(": ")
        if cqm == '1':
            time.sleep(1)
            print("The Bear notices you")
            time.sleep(1)
            print("The Bear charges towards you")
            time.sleep(1)
            print("Mountian Bear : ROAR!")
            time.sleep(1)
            print("Stabbing Barrage!")
            time.sleep(1)
            print("""You continusly stab the bear causing it to die and you to successfully complete the quest""")
            time.sleep(1)
            print("I'm going back to the adventurer's guild.")
            time.sleep(1)
            print("Receptionist : Oh, Hi {an1} did you complete the quest?")
            time.sleep(1)
            print("Yes, I did.")
            time.sleep(1)
            print("Receptionist : Alright let me have your card")
            time.sleep(1)
            print("Receptionist : Ok, So you did do complete the quest")
            time.sleep(1)
            print("Receptionist : So, here's your reward 70 Silver")
            time.sleep(1)
            print("Thanks")
            time.sleep(1)
            print("You feel dizzy as the world spins around you...")
            vision(an1, choice_skill)
        else:
            time.sleep(1)
            print("The Bear notices you")
            time.sleep(1)
            print("The Bear charges towards you")
            time.sleep(1)
            print("Mountian Bear : ROAR!")
            time.sleep(1)
            print("Slash of Destruction!")
            time.sleep(1)
            print("""You slash the bear with your sword causing it to die and you to successfully complete the quest""")
            time.sleep(1)
            print("I'm going back to the adventurer's guild.")
            time.sleep(1)
            print("Receptionist : Oh, Hi {an1} did you complete the quest?")
            time.sleep(1)
            print("Yes, I did.")
            time.sleep(1)
            print("Receptionist : Alright let me have your card")
            time.sleep(1)
            print("Receptionist : Ok, So you did do complete the quest")
            time.sleep(1)
            print("Receptionist : So, here's your reward 70 Silver")
            time.sleep(1)
            print("Thanks")
            time.sleep(1)
            print("You feel dizzy as the world spins around you...")
            vision(an1, choice_skill)
    else:
        print(f"Alright, {an1} the reward of this quest is 10 Gold")
        time.sleep(1)
        print("The Wolf was spotted roaming the forest north of the village")
        time.sleep(1)
        print("Alright I'll head there and Subjugate the Demon Wolf.")
        time.sleep(1)
        print("*Traveling to the Forest*")
        time.sleep(1)
        print("Loading...Please wait")
        time.sleep(3)
        print("You see the Demon Wolf kill 10 boars as you arive to the site.")
        time.sleep(1)
        print("Thats a Massive Woldf")
        time.sleep(1)
        print("What skill should I use")
        time.sleep(1)
        print("1 : Stabbing Barrage")
        print("2 : Slash of Destruction")
        cqm = input(": ")
        if cqm == '1':
            time.sleep(1)
            print("The Wolf notices you")
            time.sleep(1)
            print("The Wolf charges towards you")
            time.sleep(1)
            print("Demon Wolf : Growl!")
            time.sleep(1)
            print("Stabbing Barrage!")
            time.sleep(1)
            print("""You continusly stab the Wolf causing it to die and you to successfully complete the quest""")
            time.sleep(1)
            print("I'm going back to the adventurer's guild.")
            time.sleep(1)
            print("Receptionist : Oh, Hi {an1} did you complete the quest?")
            time.sleep(1)
            print("Yes, I did.")
            time.sleep(1)
            print("Receptionist : Alright let me have your card")
            time.sleep(1)
            print("Receptionist : Ok, So you did do complete the quest")
            time.sleep(1)
            print("Receptionist : So, here's your reward 10 Gold")
            time.sleep(1)
            print("Thanks")
            time.sleep(1)
            print("You feel dizzy as the world spins around you...")
            vision(an1, choice_skill)
        else:
            time.sleep(1)
            print("The Wolf notices you")
            time.sleep(1)
            print("The Wolf charges towards you")
            time.sleep(1)
            print("Demon Wolf : Growl!")
            time.sleep(1)
            print("Stabbing Barrage!")
            time.sleep(1)
            print("""You slash the Demon Wolf causing it to die and you to successfully complete the quest""")
            time.sleep(1)
            print("I'm going back to the adventurer's guild.")
            time.sleep(1)
            print("Receptionist : Oh, Hi {an1} did you complete the quest?")
            time.sleep(1)
            print("Yes, I did.")
            time.sleep(1)
            print("Receptionist : Alright let me have your card")
            time.sleep(1)
            print("Receptionist : Ok, So you did do complete the quest")
            time.sleep(1)
            print("Receptionist : So, here's your reward 10 Gold")
            time.sleep(1)
            print("Thanks")
            time.sleep(1)
            print("You feel dizzy as the world spins around you...")
            vision(an1, choice_skill)
            
def gti(an1, aa1, ap1):
    import time
    time.sleep(1)
    print("Loading...Please wait")
    print("""










        """)
    time.sleep(3)
    print("You have 10 Gold")
    time.sleep(1)
    print("Concierge : Welcome to the Pantheon Inn!")
    time.sleep(1)
    print("Hi.")
    time.sleep(1)
    print("Concierge : Are you here to check in?")
    time.sleep(1)
    print("Yes")
    time.sleep(1)
    print("Concierge : Ok, you need to fill out this form")
    time.sleep(1)
    cn = input("Name : ")
    ca = input("Age : ")
    cl = input("Length of stay : ")
    time.sleep(1)
    print("1 : Single 10 Bronze")
    print("2 : Double 10 Silver")
    print("3 : Suite 5 Gold")
    cr = input("Room Type : ")
    time.sleep(1)
    print(f"Concierge : Alright {cn} here is your room key.")
    if cr == '1':
        print("Concierge : Your room number is 5")
        time.sleep(2)
        print("The bare minimum")
        time.sleep(1)
        print("I'm going to sleep")
        time.sleep(1)
        print("*You lay on the bed*")
        time.sleep(1)
        print("As you lay on the bed you drift of to a place similar to a dreamscape")
        vision(an1, choice_skill)
    elif cr == '2':
        print("Concierge : Your room number is 15")
        time.sleep(2)
        print("This is decent")
        time.sleep(1)
        print("I'm going to rest.")
        time.sleep(1)
        print("*You lay on the bed*")
        time.sleep(1)
        print("As you lay on the bed you drift of to a place similar to a dreamscape")
        vision(an1, choice_skill)
    else:
        print("Concierge : Your room number is 30")
        time.sleep(2)
        print("This is nice")
        time.sleep(1)
        print("There's even complimentary snacks.")
        time.sleep(1)
        print("1 : Eat Snacks")
        print("2 : Go to Rest")
        rc = input(": ")
        if rc == '1':
            time.sleep(1)
            print("Lets start with these things that look like chips.")
            time.sleep(1)
            print("*Eating*")
            time.sleep(1)
            print("Wow! This tastes just like Coca Cola!")
            time.sleep(1)
            print("This is the life.")
            time.sleep(1)
            print("You drift of to a place similar to a dreamscape as you relax on your bed")
            vision(an1, choice_skill)
        else:
            time.sleep(1)
            print("I'm going to rest.")
            time.sleep(1)
            print("*You lay on the bed*")
            time.sleep(1)
            print("As you lay on the bed you drift of to a place similar to a dreamscape")
            vision(an1, choice_skill)
            
def necronq(an1):
    import time
    print("Receptionist : NECRON is a Wither King said to only awaken once every 1000 years...")
    time.sleep(1.5)
    print("Receptionist : This is the year he is said to awaken. And with that the monsters have become stronger and more violent")
    time.sleep(1)
    print("Receptionist : NECRON'S hatred to the human race has grown due to the hero that killed him 1000 years ago...")
    time.sleep(1)
    print("Receptionist : He swore to kill that hero")
    time.sleep(1)
    print(f"Receptionist : Becareful {an1}.")
    time.sleep(1)
    vision(an1, choice_skill)

def vision(an1, choice_skill):
    import time
    print("""








        """)
    print(f"Hello {an1}, sorry to take more of your time...but...")
    time.sleep(2)
    print("NECRON THE WITHER KING has awakened...you as this worlds hero will have to kill NECRON THE WITHER KING and protect the people of this world.")
    time.sleep(1)
    print("I am sorry I'm asking so much of you when you just got reincarnated in this world...")
    time.sleep(1)
    print("But, Please I beg of you save this world just like you did 1000years ago.")
    time.sleep(1)
    print("Oh, No")
    time.sleep(1)
    print("We're running out of time...I will teleport you to his dungeon...")
    time.sleep(1)
    print("To enter his dungeon you must answer a question...If you answer inccorrectly you will die")
    time.sleep(1)
    print("Becareful Hero")
    time.sleep(3)
    print("Loading...Please wait")
    maxor(an1, choice_skill)
def stv():
    import time
    print("Loading...Please wait")
    time.sleep(3)
    print("Wow, so much food")
    time.sleep(1)
    print("Knight : Hey! You!")
    time.sleep(1)
    print("Knight : Who are you! You don't have identification")
    time.sleep(1)
    print("Who? Me?")
    time.sleep(1)
    print("Knight : Yes you!")
    time.sleep(1)
    print("But the Guard at the gate said that all I had to do is to hover my hand over a magic ball")
    time.sleep(1)
    print("Knight : Oh...Sorry for my mistake.")
    time.sleep(1)
    print("Knight : You should go make an identification card at the Guild so the knights won't be alerted.")
    time.sleep(1)
    print("Oh ok.")
    time.sleep(1)
    print("Knight : I could bring you there")
    time.sleep(1)
    print("Sure")
    time.sleep(1)
    print("*Entering Adventurers Guild*")
    time.sleep(1)
    print("Loading...Please wait")
    time.sleep(3)
    print("Knight : Alright, here we are.")
    time.sleep(1)
    print("Thanks for bringing me here")
    time.sleep(1)
    print("Knight : No problem.")
    gag()

def necron_fight(an1, choice_skill):
    global health
    health = '5000'
    stamina = '5000'
    mana = '2500'
    global sworddmg
    sworddmg = '100000'
    global staffdmg
    staffdmg = '200000'
    necron_health = '1000000'

    
    print("""












        """)

    print("NECRON : HERO YOU KILLED ME BEFORE AND NOW YOU COME IN MY DOMAIN AND KILL ALL THREE OF MY SONS!")
    time.sleep(1)
    print("NECRON : YOU WILL PAY FOR YOUR ACTIONS AGAINST MY EMPIRE")
    time.sleep(2)
    if choice_skill == '1':
        global stamina1
        stamina1 = '5000'
        global mana1
        mana1 = '5000'
        print(f"Aionia : You have Health : {health} , Stamina : {stamina1} , Mana : {mana1} .")
        time.sleep(2)
        print(f"Aionia : Goodluck {an1} be careful in this fight NECRON isn't easy to defeat")
        time.sleep(1)
        print("NECRON : COME AT ME COWARD!")
        time.sleep(1)
        print("NECRON HEALTH : 1M")
        time.sleep(1)
        print("NECRON shoots a wither skull at you dealing 500 damage")
        time.sleep(1)
        print(f"{an1}, you have 4500hp")
        time.sleep(1)
        print("1 : Fire Ball : Deals 300000 , Mana Cost : 2000")
        time.sleep(1)
        print("2 : Water Slash : Deals 150000 , Mana Cost : 900")
        fa = input(": ")
        if fa == '1':
            print("NECRON HEALTH : 700K")
            time.sleep(1)
            print("NECRON : YOU DARE ATTACK ME! TAKE THIS!")
            time.sleep(1)
            print("NECRON shoots a beam of acid at you dealing 1000 damage")
            time.sleep(1)
            print(f"{an1}, you have 3500hp")
            time.sleep(1)
            print("You remember what caused you to fight against NECRON to begin with.")
            time.sleep(1)
            print("You think as you remember NECRON ravaged your village killing your family in front of you")
            time.sleep(1)
            print("Anger boils up inside you as you remember that day as if it was yesterday.")
            time.sleep(1)
            print("NECRON YOU BASTARD. YOU KILLED MY FAMILY I WILL KILL YOU AGAIN JUST LIKE I DID A MILLENNIA AGO!")
            time.sleep(1)
            print("TIME TO END THIS!")
            time.sleep(1)
            print("You cast Rain of Annihilation killing NECRON in one blast")
            time.sleep(1)
            print("NECRON : NOOOO! I HAVE FAILED TWICE MOTHER FORGIVE ME!")
            time.sleep(1)
            print("AIONIA : HERO YOU DARE KILL MY SON AND MY GRANDSONS!")
            time.sleep(1)
            print("AIONIA : COME FACE ME")
            time.sleep(1)
            print("Aionia? Your NECRON's mother? But you helped me?")
            time.sleep(1)
            print("AIONIA : I ONLY HELPED YOU BECAUSE I WANTED TO TEST MY SON!")
            time.sleep(1)
            print("AIONIA hit you with her ultimate attack leaving you with 100hp")
            time.sleep(1)
            print("""In that moment the power from your ancestors surged within you providing you with power,allowing you to attack AIONIA with your
                  ultimate spell""")
            time.sleep(1)
            print("Existence Eraser")
            time.sleep(1)
            print("With that skill you killed AIONIA with one attack")
            print("AIONIA : NOOOO!")
            time.sleep(3)
            print("AMC : Thank You hero for getting rid of that pest.")
            time.sleep(1)
            print("AMC : I am truly grateful and as a reward I will return you to your previous world.")
            time.sleep(3)
            print("""









                """)
            print("You wake up in a hospital thinking the events that occured was just a dream...but was it?")
            time.sleep(3)
            print("It's been 3 years and I still wonder if the dream I had at the hospital was actually a dream...")
            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0)
        else:
            print("NECRON HEALTH : 850K")
            time.sleep(1)
            print("NECRON : YOU DARE ATTACK ME! TAKE THIS!")
            time.sleep(1)
            print("NECRON shoots a beam of acid at you killing you instantly")
            time.sleep(1)
            print("NECRON : FINALLY MOTHER I SUCCEEDED IN KILLING THE HERO!")
            time.sleep(1)
            print("AIONIA : Good my son...")
            time.sleep(2)
            print(r"""

                  ____    _    __  __ _____    _____     _______ ____  
                 / ___|  / \  |  \/  | ____|  / _ \ \   / / ____|  _ \ 
                | |  _  / _ \ | |\/| |  _|   | | | \ \ / /|  _| | |_) |
                | |_| |/ ___ \| |  | | |___  | |_| |\ V / | |___|  _ < 
                 \____/_/   \_\_|  |_|_____|  \___/  \_/  |_____|_| \_\


                """)
            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0)
    else:
        global stamina2
        stamina2 = '10000'
        global health1
        health1 = '10000'
        print(f"Aionia : You have {health1} , {stamina2} , {mana} .")
        time.sleep(2)
        print(f"Aionia : Goodluck {an1} be careful in this fight NECRON isn't easy to defeat")
        time.sleep(1)
        print("NECRON : COME AT ME COWARD!")
        time.sleep(1)
        print("NECRON HEALTH : 1M")
        time.sleep(1)
        print("NECRON shoots a wither skull at you dealing 1000 damage")
        print(f"{an1}, you have 9000hp")
        time.sleep(1)
        print("1 : Compound Slash : Deals 400000 , Stamina Cost 2000")
        print("2 : Incessant Incisions : Deals 300000 , Stamina Cost 1600")
        fa = input(": ")
        if fa == '1':
            print("NECRON HEALTH : 600K")
            time.sleep(1)
            print("NECRON : YOU DARE ATTACK ME! TAKE THIS!")
            time.sleep(1)
            print("NECRON shoots a beam of acid at you dealing 3000 damage")
            time.sleep(1)
            print(f"{an1}, you have 6000hp")
            time.sleep(1)
            print("You remember what caused you to fight against NECRON to begin with.")
            time.sleep(1)
            print("You think as you remember NECRON ravaged your village killing your family in front of you")
            time.sleep(1)
            print("Anger boils up inside you as you remember that day as if it was yesterday.")
            time.sleep(1)
            print("NECRON YOU BASTARD. YOU KILLED MY FAMILY I WILL KILL YOU AGAIN JUST LIKE I DID A MILLENNIA AGO!")
            time.sleep(1)
            print("TIME TO END THIS!")
            time.sleep(1)
            print("You attack NECRON with Slash of Annihilation")
            time.sleep(1)
            print("NECRON : NOOOO! I HAVE FAILED TWICE MOTHER FORGIVE ME!")
            time.sleep(1)
            print("Accidentally, you hurt NECRON'S Mother AIONIA.")
            time.sleep(1)
            print("AIONIA : HERO YOU KILLED MY SON AND GRANDSONS AND THEN YOU HAVE THE AUDACITY TO COME AND ATTACK ME.")
            time.sleep(1)
            print("What? Your NECRON'S mother?")
            time.sleep(1)
            print("But you helped me.")
            time.sleep(1)
            print("AIONIA : I ONLY DID THAT TO TEST MY SON NOT TO KILL HIM!")
            time.sleep(1)
            print("AIONIA : NOW THAT YOU'VE COMMITTED THIS ACT I WILL END YOU!")
            time.sleep(1)
            print("""In that moment the power from your ancestors surged within you providing you with power,allowing you to attack AIONIA with your
                  ultimate move""")
            time.sleep(1)
            print("JUDGMENT")
            time.sleep(1)
            print("AIONIA : NOOOO!")
            time.sleep(3)
            print("AMC : Thank You hero for getting rid of that pest.")
            time.sleep(1)
            print("AMC : I am truly grateful and as a reward I will return you to your previous world.")
            time.sleep(3)
            print("""









                """)
            print("You wake up in a hospital thinking the events that occured was just a dream...but was it?")
            time.sleep(3)
            print("It's been 3 years and I still wonder if the dream I had at the hospital was actually a dream...")
            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0)
        else:
            print("You get up as you failed to attack NECRON.")
            time.sleep(1)
            print("No...It cant be.")
            time.sleep(1)
            print("NECRON : YES HERO YOU LOST I WON MOTHER !")
            time.sleep(1)
            print("AIONIA : Well done my son")
            time.sleep(2)
            print(r"""

                  ____    _    __  __ _____    _____     _______ ____  
                 / ___|  / \  |  \/  | ____|  / _ \ \   / / ____|  _ \ 
                | |  _  / _ \ | |\/| |  _|   | | | \ \ / /|  _| | |_) |
                | |_| |/ ___ \| |  | | |___  | |_| |\ V / | |___|  _ < 
                 \____/_/   \_\_|  |_|_____|  \___/  \_/  |_____|_| \_\


                """)
            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0) 

def goldor(an1, choice_skill):
    print("""












        """)
    print(f"Goldor : {an1} you killed 2 of my brothers I will end you for your actions.")
    time.sleep(1)
    print("Goldor : Answer this riddle.")
    if choice_skill == '1':
        print("If a hen and a half lay an egg and a half in a day and a half, how many eggs will half a dozen hens lay in half a dozen days?")
        mage_question = input(": ")
        if mage_question == '24':
            print("Goldor : Noooo! FATHER I FAILED! BROTHERS I'M SORRY!")
            time.sleep(1)
            print("NECRON : HERO YOU KILLED ALL 3 OF MY SONS! COME FACE ME COWARD")
            necron_fight(an1, choice_skill)
        else:
            print(f"Goldor : Father I defeated the hero. Brothers you can now rest in peace.")
            time.sleep(1)
            print("NECRON : Well done my son...")
            time.sleep(1)
            print(r"""

                  ____    _    __  __ _____    _____     _______ ____  
                 / ___|  / \  |  \/  | ____|  / _ \ \   / / ____|  _ \ 
                | |  _  / _ \ | |\/| |  _|   | | | \ \ / /|  _| | |_) |
                | |_| |/ ___ \| |  | | |___  | |_| |\ V / | |___|  _ < 
                 \____/_/   \_\_|  |_|_____|  \___/  \_/  |_____|_| \_\


                """)

            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0)
    
    else:
        
        print("What is the smallest whole number that is equal to seven times the sum of its digits?")
        sword_question = input(": ")
        if sword_question == '21':
            print("Goldor : Noooo! FATHER FORGIVE ME! BROTHERS I'M SORRY")
            time.sleep(1)
            print("NECRON : YOU DARE HERO! YOU KILLED ALL 3 OF MY SONS! COME FACE ME LIKE A MAN YOU COWARD")
            necron_fight(an1, choice_skill)
        else:
            print(f"Goldor : Father the Hero is dead")
            time.sleep(1)
            print("NECRON : Well done my son...")
            time.sleep(1)
            print(r"""

                  ____    _    __  __ _____    _____     _______ ____  
                 / ___|  / \  |  \/  | ____|  / _ \ \   / / ____|  _ \ 
                | |  _  / _ \ | |\/| |  _|   | | | \ \ / /|  _| | |_) |
                | |_| |/ ___ \| |  | | |___  | |_| |\ V / | |___|  _ < 
                 \____/_/   \_\_|  |_|_____|  \___/  \_/  |_____|_| \_\


                """)

            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0)
        

def storm(an1, choice_skill):
    print("""












        """)
    print(f"Storm : {an1} how dare you try challange father.")
    time.sleep(1)
    print("You don't scare me Storm.")
    time.sleep(1)
    print("Storm : In your dreams.")
    time.sleep(1)
    print("Storm : To continue you have to solve this problem.")
    time.sleep(1)
    if choice_skill == '1':
        print("Calculate the hypotenuse of the triangle where a = 3 and b = 4")
        mage_question = input("c = ")
        if mage_question == '5':
            print("Storm : Noooo! FATHER FORGIVE ME!")
            time.sleep(1)
            print("NECRON : HERO YOU DARE CHALLENGE ME!")
            goldor(an1, choice_skill)
        else:
            print(f"Storm : Father I defeated the hero.")
            time.sleep(1)
            print("NECRON : Well done my son...")
            time.sleep(1)
            print(r"""

                  ____    _    __  __ _____    _____     _______ ____  
                 / ___|  / \  |  \/  | ____|  / _ \ \   / / ____|  _ \ 
                | |  _  / _ \ | |\/| |  _|   | | | \ \ / /|  _| | |_) |
                | |_| |/ ___ \| |  | | |___  | |_| |\ V / | |___|  _ < 
                 \____/_/   \_\_|  |_|_____|  \___/  \_/  |_____|_| \_\


                """)

            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0)
    
    else:
        
        print("Solve this quadratic equation '2x^2 + 3x - 2 = 0' using the quadratic formula")
        print("Write the positive answer as either a whole number or decimal")
        sword_question = input("x = ")
        if sword_question == '0.5':
            print("Storm : Noooo! FATHER FORGIVE ME!")
            time.sleep(1)
            print("NECRON : YOU DARE HERO!")
            goldor(an1, choice_skill)
        else:
            print(f"Storm : Father the Hero is dead")
            time.sleep(1)
            print("NECRON : Well done my son...")
            time.sleep(1)
            print(r"""

                  ____    _    __  __ _____    _____     _______ ____  
                 / ___|  / \  |  \/  | ____|  / _ \ \   / / ____|  _ \ 
                | |  _  / _ \ | |\/| |  _|   | | | \ \ / /|  _| | |_) |
                | |_| |/ ___ \| |  | | |___  | |_| |\ V / | |___|  _ < 
                 \____/_/   \_\_|  |_|_____|  \___/  \_/  |_____|_| \_\


                """)

            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0)
        
def maxor(an1, choice_skill):
    
    if choice_skill == '1':
        character_id = '1'
    else:
        character_id = '2'
    print("""












        """)
    print("Maxor : Ah...The Hero...")
    time.sleep(1.5)
    print("Maxor : You dare show your face around here again after you defeated my Master...")
    time.sleep(1.5)
    print("*You start to regain your memories*")
    time.sleep(0.5)
    print("I will save this world at all costs")
    time.sleep(1)
    print("Maxor : Very well Hero...")
    time.sleep(1.5)
    print("Maxor : You have to go through me first")
    time.sleep(2)
    if character_id == '1':
        print(f"Maxor : Ok. an1 answer this riddle.")
        time.sleep(2)
        print("What are the next three letters in this combination? OTTFFSS")
        time.sleep(1)
        print("Write your answer with spaces in between them and the letters have to be capitalized.")
        riddle_mage = input(": ")
        if riddle_mage == 'E N T':
            print(f"Maxor : Noooo!Father I failed.")
            time.sleep(1)
            storm(an1, choice_skill)
            
        else:
            print(f"Maxor : Father...I killed the Hero")
            time.sleep(1)
            print("NECRON : Well done my son...")
            print(r"""

                  ____    _    __  __ _____    _____     _______ ____  
                 / ___|  / \  |  \/  | ____|  / _ \ \   / / ____|  _ \ 
                | |  _  / _ \ | |\/| |  _|   | | | \ \ / /|  _| | |_) |
                | |_| |/ ___ \| |  | | |___  | |_| |\ V / | |___|  _ < 
                 \____/_/   \_\_|  |_|_____|  \___/  \_/  |_____|_| \_\


                """)

            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0)
    else:
        print(f"Maxor : Ok. an1 answer this riddle.")
        time.sleep(2)
        print("If the English alphabet goes from A to Z, what goes from Z to A?")
        time.sleep(1)
        print("Write your answer capitalized the correct way.")
        riddle_swordsman = input(": ")
        riddle = riddle_swordsman.capitalize
        if riddle == 'Zebra':
            print(f"Maxor : Noooo...Father I failed.")
            time.sleep(1)
            storm(an1, choice_skill)
            
        else:
            print(f"Maxor : Father...I have avenged you...")
            time.sleep(1)
            print("NECRON : Well done my son...")
            time.sleep(1)
            print(r"""

                  ____    _    __  __ _____    _____     _______ ____  
                 / ___|  / \  |  \/  | ____|  / _ \ \   / / ____|  _ \ 
                | |  _  / _ \ | |\/| |  _|   | | | \ \ / /|  _| | |_) |
                | |_| |/ ___ \| |  | | |___  | |_| |\ V / | |___|  _ < 
                 \____/_/   \_\_|  |_|_____|  \___/  \_/  |_____|_| \_\


                """)
            time.sleep(2)
            print("1 : Return to Main Menu")
            time.sleep(1)
            print("2 : Replay")
            time.sleep(1)
            print("3 : Leave Game")
            time.sleep(1)
            wwy = str(input(": "))
            if wwy == '1':
                main()
            elif wwy == '2':
                GOM()
            else:
                sys.exit(0)
            
def enigmadigits():
            import time
            import random
            status = str('running')
            gid = str('2')
            def guess_the_number():
                secret_number = random.randint(1,100)

                attempts = 0
                max_attempts = 10


                print(r"""


                     _____       _                       ____  _       _ _       
                    | ____|_ __ (_) __ _ _ __ ___   __ _|  _ \(_) __ _(_) |_ ___ 
                    |  _| | '_ \| |/ _` | '_ ` _ \ / _` | | | | |/ _` | | __/ __|
                    | |___| | | | | (_| | | | | | | (_| | |_| | | (_| | | |_\__ \
                    |_____|_| |_|_|\__, |_| |_| |_|\__,_|____/|_|\__, |_|\__|___/
                                    |___/                         |___/


                        """)      
                
                print("Please wait...")
                time.sleep(3)
                print("Welcome to the Guess the Number game!")
                print("I'm thinking of a number between 1 and 100.")
                

                while attempts < max_attempts :
                    try:
                        
                        guess = int(input("Your guess : "))

                        if guess < 1 or guess > 1000 :
                            print("Please guess a number between 1 and 100.")
                            continue

                        attempts += 1

                        if guess < secret_number :
                            print("Too low! Try again.")
                        elif guess > secret_number :
                            print("Too high! Try again.")
                        else:
                            status = str('ended')
                            print(f"Congratulations! You guessed the number {secret_number} in {attempts} attempts")
                            
                    except ValueError:
                        print("Invalid input. Please enter a valid number.")

                if attempts ==  max_attempts:
                    status = str('ended')
                    print(f"Sorry, you've reached the maximum number of attempts. The secret number was {secret_number}.")
                    
                    
                        
            if __name__=="__main__" :
                guess_the_number()
     
import time
import sys
print("Loading...Please wait")
time.sleep(3)
print()
print()
print()
print("UnityGrid Access version : 1.0")
time.sleep(1)
print("Made by Virtual Vanguard Studios")
time.sleep(2)
print(r"""


         _   _       _ _          ____      _     _      _                         
        | | | |_ __ (_) |_ _   _ / ___|_ __(_) __| |    / \   ___ ___ ___  ___ ___ 
        | | | | '_ \| | __| | | | |  _| '__| |/ _` |   / _ \ / __/ __/ _ \/ __/ __|
        | |_| | | | | | |_| |_| | |_| | |  | | (_| |  / ___ \ (_| (_|  __/\__ \__ \
         \___/|_| |_|_|\__|\__, |\____|_|  |_|\__,_| /_/   \_\___\___\___||___/___/
                           |___/

                           
        """)


print("Welcome to UntiyGrid Access!")




def readdb():
    with open('database.txt', 'r') as f:
        contents = f.readlines()

        newc = []


        for line in contents:
            fields = line.split(',')
            fields[1] = fields[1].rstrip()
            newc.append(fields)
        return newc

logins = readdb()

def login():
    username = str(input("Username : "))
    password = str(input("Password : "))
    username1 = username.capitalize()

    logged_in = False

    for line in logins:
        if line[0] == username and logged_in == False:
            if line[1] == password:
                logged_in = True
    if logged_in == True:
        
        main()
        
    else:
        print("Incorrect Username or Password was inputed")
        print("Please Try Again")
        login()


login()
