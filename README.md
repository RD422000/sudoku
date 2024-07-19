# sudoku
Explanation:
print_board(board):

Prints the Sudoku board. Zeros are replaced with dots for better readability.
find_empty_location(board):

Finds an empty location (represented by 0) in the board and returns its coordinates as a tuple (row, col). If no empty location is found, it returns None.
is_valid(board, num, pos):

Checks if placing num at the position pos is valid according to Sudoku rules:
Checks the row, column, and 3x3 box to ensure the number is not repeated.
solve_sudoku(board):

Uses the backtracking algorithm to solve the Sudoku puzzle:
Finds an empty location.
Tries placing numbers 1 to 9 in the empty location.
If the number is valid, it places the number and recursively tries to solve the rest of the board.
If placing the number doesn't lead to a solution, it backtracks and tries the next number.
if __name__ == "__main__"::

Initializes a sample Sudoku board.
Prints the original board.
Attempts to solve the board and prints the result. If no solution exists, it informs the user.
