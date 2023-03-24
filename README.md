# jk_flip_flop
#CODE; JK FLIP FLOP 


# initialize variables
Q = 0
Q_bar = 1
J = 0
K = 0

# define the flip flop function
def jk_flip_flop(J, K, Q, Q_bar):
    if J == 1 and K == 0:
        Q = 1
        Q_bar = 0
    elif J == 0 and K == 1:
        Q = 0
        Q_bar = 1
    elif J == 1 and K == 1:
        Q = 1 - Q
        Q_bar = 1 - Q_bar
    return Q, Q_bar

# test the flip flop function
J = 1
K = 0
Q, Q_bar = jk_flip_flop(J, K, Q, Q_bar)
print("Q:", Q, "Q_bar:", Q_bar)

J = 0
K = 1
Q, Q_bar = jk_flip_flop(J, K, Q, Q_bar)
print("Q:", Q, "Q_bar:", Q_bar)

J = 1
K = 1
Q, Q_bar = jk_flip_flop(J, K, Q, Q_bar)
print("Q:", Q, "Q_bar:", Q_bar)

J = 0
K = 0
Q, Q_bar = jk_flip_flop(J, K, Q, Q_bar)
print("Q:", Q, "Q_bar:", Q_bar)
