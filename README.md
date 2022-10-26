import random
from colorama import Fore, Style
import time

start=time.time()

nun=[['_','_','_'],['_','_','_'],['_','_','_']]


for i in range(3):
    for j in range(3):
        print(nun[i][j],end=' ')
    print('')

choice=[0,1,2]

Pc_user=int(input('entre 1 to play with pc or 2 to play with your firend:'))

while True:
    
    if Pc_user==1:

        while True:
            print('user turn:')
            Ucolumn=int(input('entre sootoon number:'))
            URow=int(input('enre radif:'))
            if Ucolumn>=0 and Ucolumn<3 and URow>=0 and URow<3 and nun[Ucolumn] [URow]=='_':
                nun[Ucolumn] [URow]=Fore.GREEN+'X'+Fore.RESET
                for i in range(3):
                    for j in range(3):
                        print(nun[i][j],end=' ')
                    print('')

                break
            else:
                print(' fals address , Try agin ')
        

        if nun[0][0]==Fore.GREEN+'X'+Fore.RESET and nun[0][1]==Fore.GREEN+'X'+Fore.RESET and nun[0][2]==Fore.GREEN+'X'+Fore.RESET:
            print('user is winner')
            break
        
        if nun[1][0]==Fore.GREEN+'X'+Fore.RESET and nun[1][1]==Fore.GREEN+'X'+Fore.RESET and nun[1][2]==Fore.GREEN+'X'+Fore.RESET:
            print('user is winner')
            break
        if nun[2][0]==Fore.GREEN+'X'+Fore.RESET and nun[2][1]==Fore.GREEN+'X'+Fore.RESET and nun[2][2]==Fore.GREEN+'X'+Fore.RESET:
            print('user is winner')
            break
        if nun[0][0]==Fore.GREEN+'X'+Fore.RESET and nun[1][0]==Fore.GREEN+'X'+Fore.RESET and nun[2][0]==Fore.GREEN+'X'+Fore.RESET:
            print('user is winner')
            break
        if nun[0][1]==Fore.GREEN+'X'+Fore.RESET and nun[1][1]==Fore.GREEN+'X'+Fore.RESET and nun[2][1]==Fore.GREEN+'X'+Fore.RESET:
            print('user is winner')
            break
        if nun[0][2]==Fore.GREEN+'X'+Fore.RESET and nun[1][2]==Fore.GREEN+'X'+Fore.RESET and nun[2][2]==Fore.GREEN+'X'+Fore.RESET:
            print('user is winner')
            break
        if nun[0][0]==Fore.GREEN+'X'+Fore.RESET and nun[1][1]==Fore.GREEN+'X'+Fore.RESET and nun[2][2]==Fore.GREEN+'X'+Fore.RESET:
            print('user is winner')
            break
        if nun[0][2]==Fore.GREEN+'X'+Fore.RESET and nun[1][1]==Fore.GREEN+'X'+Fore.RESET and nun[2][0]=='X':
            print('user is winner')
            break
        while True:
            print('pc turn')
            Pcolumn=random.choice(choice)
            Prow=random.choice(choice)
            if Pcolumn>=0 and Pcolumn<3 and Prow>=0 and Prow<3 and nun[Pcolumn][Prow]=='_':
                nun[Pcolumn][Prow]=Fore.RED+'O'+Style.RESET_ALL
                for i in range(3):
                    for j in range(3):
                        print(nun[i][j],end=' ')
                    print('')
                break
            else:
                print(' fals address , Try agin ')
        if nun[0][0]==Fore.RED+'O'+Style.RESET_ALL and nun[0][1]==Fore.RED+'O'+Style.RESET_ALL and nun[0][2]=='O':
            print('pc is winner')
            break
        if nun[1][0]==Fore.RED+'O'+Style.RESET_ALL and nun[1][1]=='O' and nun[1][2]=='O':
            print('pc is winner')
            break
        if nun[2][0]==Fore.RED+'O'+Style.RESET_ALL and nun[2][1]==Fore.RED+'O'+Style.RESET_ALL and nun[2][2]==Fore.RED+'O'+Style.RESET_ALL:
            print('pc is winner')
            break
        if nun[0][0]==Fore.RED+'O'+Style.RESET_ALL and nun[1][0]==Fore.RED+'O'+Style.RESET_ALL and nun[2][0]==Fore.RED+'O'+Style.RESET_ALL:
            print('pc is winner')
            break
        if nun[0][1]==Fore.RED+'O'+Style.RESET_ALL and nun[1][1]==Fore.RED+'O'+Style.RESET_ALL and nun[2][1]==Fore.RED+'O'+Style.RESET_ALL:
            print('pc is winner')
            break
        if nun[0][2]==Fore.RED+'O'+Style.RESET_ALL and nun[1][2]==Fore.RED+'O'+Style.RESET_ALL and nun[2][2]==Fore.RED+'O'+Style.RESET_ALL:
            print('pc is winner')
            break
        if nun[0][0]==Fore.RED+'O'+Style.RESET_ALL and nun[1][1]==Fore.RED+'O'+Style.RESET_ALL and nun[2][2]==Fore.RED+'O'+Style.RESET_ALL:
            print('pc is winner')
            break
        if nun[0][2]==Fore.RED+'O'+Style.RESET_ALL and nun[1][1]==Fore.RED+'O'+Style.RESET_ALL and nun[2][0]==Fore.RED+'O'+Style.RESET_ALL:
            print('pc is winner')
            break
        elif '_' not in nun:
            print("mosavi")
    if Pc_user==2:
        while True:
            print('player1 turn:')
            Ucolumn=int(input('entre sootoon number:'))
            URow=int(input('enre radif:'))
            if Ucolumn>=0 and Ucolumn<3 and URow>=0 and URow<3 and nun[Ucolumn] [URow]=='_':
                nun[Ucolumn] [URow]=Fore.GREEN+'X'+Fore.RESET
                for i in range(3):
                    for j in range(3):
                        print(nun[i][j],end=' ')
                    print('')

                break
            else:
                print(' fals address , Try agin ')
        

        if nun[0][0]==Fore.GREEN+'X'+Fore.RESET and nun[0][1]==Fore.GREEN+'X'+Fore.RESET and nun[0][2]==Fore.GREEN+'X'+Fore.RESET:
            print('player1 is winner')
            break
        if nun[1][0]==Fore.GREEN+'X'+Fore.RESET and nun[1][1]==Fore.GREEN+'X'+Fore.RESET and nun[1][2]==Fore.GREEN+'X'+Fore.RESET:
            print('player1 is winner')
            break
        if nun[2][0]==Fore.GREEN+'X'+Fore.RESET and nun[2][1]==Fore.GREEN+'X'+Fore.RESET and nun[2][2]==Fore.GREEN+'X'+Fore.RESET:
            print('player1 is winner')
            break
        if nun[0][0]==Fore.GREEN+'X'+Fore.RESET and nun[1][0]==Fore.GREEN+'X'+Fore.RESET and nun[2][0]==Fore.GREEN+'X'+Fore.RESET:
            print('player1 is winner')
            break
        if nun[0][1]==Fore.GREEN+'X'+Fore.RESET and nun[1][1]==Fore.GREEN+'X'+Fore.RESET and nun[2][1]==Fore.GREEN+'X'+Fore.RESET:
            print('player1 is winner')
            break
        if nun[0][2]==Fore.GREEN+'X'+Fore.RESET and nun[1][2]==Fore.GREEN+'X'+Fore.RESET and nun[2][2]==Fore.GREEN+'X'+Fore.RESET:
            print('player1 is winner')
            break
        if nun[0][0]==Fore.GREEN+'X'+Fore.RESET and nun[1][1]==Fore.GREEN+'X'+Fore.RESET and nun[2][2]==Fore.GREEN+'X'+Fore.RESET:
            print('player1 is winner')
            break
        if nun[0][2]==Fore.GREEN+'X'+Fore.RESET and nun[1][1]==Fore.GREEN+'X'+Fore.RESET and nun[2][0]==Fore.GREEN+'X'+Fore.RESET:
            print('player1 is winner')
            break
        
        while True:
            print('player2 turn')
            Pcolumn=int(input('entre sootoon number:'))
            Prow=int(input('entre radif number:'))
            if Pcolumn>=0 and Pcolumn<3 and Prow>=0 and Prow<3 and nun[Pcolumn][Prow]=='_':
                nun[Pcolumn][Prow]=Fore.RED+'O'+Style.RESET_ALL
                for i in range(3):
                    for j in range(3):
                        print(nun[i][j],end=' ')
                    print('')
                break
            else:
                print(' fals address , Try agin ')
        if nun[0][0]==Fore.RED+'O'+Style.RESET_ALL and nun[0][1]==Fore.RED+'O'+Style.RESET_ALL and nun[0][2]==Fore.RED+'O'+Style.RESET_ALL:
            print('player2 is winner')
            break
        if nun[1][0]==Fore.RED+'O'+Style.RESET_ALL and nun[1][1]==Fore.RED+'O'+Style.RESET_ALL and nun[1][2]==Fore.RED+'O'+Style.RESET_ALL:
            print('player2 is winner')
            break
        if nun[2][0]==Fore.RED+'O'+Style.RESET_ALL and nun[2][1]==Fore.RED+'O'+Style.RESET_ALL and nun[2][2]==Fore.RED+'O'+Style.RESET_ALL:
            print('player2 is winner')
            break
        if nun[0][0]==Fore.RED+'O'+Style.RESET_ALL and nun[1][0]==Fore.RED+'O'+Style.RESET_ALL and nun[2][0]==Fore.RED+'O'+Style.RESET_ALL:
            print('player2 is winner')
            break
        if nun[0][1]==Fore.RED+'O'+Style.RESET_ALL and nun[1][1]==Fore.RED+'O'+Style.RESET_ALL and nun[2][1]==Fore.RED+'O'+Style.RESET_ALL:
            print('player2 is winner')
            break
        if nun[0][2]==Fore.RED+'O'+Style.RESET_ALL and nun[1][2]==Fore.RED+'O'+Style.RESET_ALL and nun[2][2]==Fore.RED+'O'+Style.RESET_ALL:
            print('player2 is winner')
            break
        if nun[0][0]==Fore.RED+'O'+Style.RESET_ALL and nun[1][1]==Fore.RED+'O'+Style.RESET_ALL and nun[2][2]==Fore.RED+'O'+Style.RESET_ALL:
            print('player2 is winner')
            break
        if nun[0][2]==Fore.RED+'O'+Style.RESET_ALL and nun[1][1]==Fore.RED+'O'+Style.RESET_ALL and nun[2][0]==Fore.RED+'O'+Style.RESET_ALL:
            print('player2 is winner')
            break
        elif '_' not in nun:
            print("mosavi")
print('Ended after:',int(time.time()-start),'s')

