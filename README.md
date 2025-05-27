Download link : 

Exercise – Week 2: LSQFit in Python
Be prepared for the exercise sessions (watch the demo lecture). You may ask TAs to help if you cannot make your program to work, but don’t expect them to show you how to start from the scratch.

    Linear model t with N > 2 training points (30 points)

        During the lecture we started to derive solutions for the parameters a and b of the linear model y = ax + b and for N training samples f(x1; y1); (x2; y2); : : : ; (xN; yN)g.

You should rst nish the derivation. Do not google, but allow yourself to do the math since errors will be found in the next steps.

        Implement a Python function my lin t(x,y) that solves and returns a and b. Use your own derivations in the function – no matter how \ugly” they are – to convince yourself about your super powers.

        Write a Python program that asks user to give N points with a mouse (left click: add point, right

click: stop collecting) and then plots the points and a tted linear model. (dataml100)$ python fit_line.py

You may start with this code snippet or write your own:

# L i n e a r s o l v e r

def m y l i n f i t ( x , y ) :

a = 0

b = 0

return a , b

    # Main
    				

    import m a t p l o t l i b . p y p l o t
    	

    a s p l t

    import numpy a s np
    				

    x = np . random . uniform (
    	

    2 ,5 ,10)

    y = np . random . uniform ( 0 , 3 , 1 0 )

    a , b = m y l i n f i t ( x , y )
    				

    p l t . p l o t ( x , y , ’ kx ’ )
    				

    xp = np . a r a n g e ( 2 , 5 , 0 . 1 )
    			

    p l t . p l o t ( xp , a∗xp+b , ’ r
    	

    ’ )
    			

    print ( f “My
    		

    f i t :
    		

    a=fbg
    		

    and
    			

    b=fbg” )

    p l t . show ( )
    				

Return the following items:

    Python code: <surname> t line.py

    A full desktop screenshot that includes the terminal window or IDE for code execution and the plot window after line tting:

<surname> t line screenshot.png

1
