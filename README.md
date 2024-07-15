# Karel-walks-around-the-world
from karel.stanfordkarel import *

def main():
    box_beepers()
    three_turn()
    two_turn()
    
def two_turn():
    turn_left()
    turn_left()

def three_turn():
    for i in range(3):
        turn_left()
            
def box_beepers():
    putting_beepers_empty()
    turn_left()
    putting_beepers_empty()
    turn_left()
    putting_beepers_empty()
    turn_left()
    putting_beepers_empty()

def putting_beepers_empty():
    if no_beepers_present():
        while front_is_clear():
            #move()
            put_beeper()
            move()
        


# don't change this code
if __name__ == '__main__':
    main()
