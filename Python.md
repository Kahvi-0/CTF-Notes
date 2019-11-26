## pwn
#refernece https://www.youtube.com/watch?v=UhbCDhHZeqY for one of the picoCTF challenges

#http://docs.pwntools.com/en/stable/

#http://docs.pwntools.com/en/stable/intro.html#making-connections

#http://docs.pwntools.com/en/stable/install.html

https://github.com/Gallopsled/pwntools-tutorial

https://github.com/Gallopsled/pwntools-tutorial/blob/master/tubes.md

    pip install pwn

    from pwn import *

## Convertion:

    "<hex>".decode("hex")
 
 
    Decimal to binary 
 
    bin(<decimal>)
    
  ### Binary to ascii
    
    n = int('011001100110000101101100011000110110111101101110', 2)
    n.to_bytes((n.bit_length() + 7) // 8, 'big').decode()

    binascii.    (https://docs.python.org/2/library/binascii.html)


## Network connections

http://docs.pwntools.com/en/stable/intro.html

    conn = ('<address>', <port>)

    conn.recvline()  #one line at a time
    
    conn.recvuntil()
