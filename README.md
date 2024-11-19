~CS431 Assignment 3 for Team 10; Brandon, Kevin, and Rebecca ~DUE ON: Tuesday Decenmber 3rd, 2024 at 12:00 midnight

The purpose of this project is first for you to show that you can express practical programming  
features as lambda expressions.  Recall that the two concepts of lambda abstraction (anonymous  
(lambda) functions) and lambda application (applying lambda functions to some argument(s)) 
are enough to compute anything you can possibly compute mechanically (say by computers). 
Second, you have to show that you can actually do proofs of correctness, as per my CLASS 20 
slides, using structural induction. 

1.  Given lambda expressions A and B,  show a lambda expression for 
if   
A  then  false   else  B 
Simplify (i.e. apply any feasible -reduction) as much as possible. 
2.  Given lambda expressions A and B,   show a lambda expression for 
A  implies  (not B) 
Simplify (i.e. apply any feasible -reduction) as much as possible. 
Hint:   What is ‘implies’ in terms of  not/or? 
Of course, you may use whatever is relevant from the CLASS 18 slides. 
3.  Given lambda expressions A and B,   show a lambda expression for 
                                A   XOR   B   (A  exclusive-OR  B) 
           Simplify (i.e. apply any feasible -reduction) as much as possible. 
 
       Hint:   What is ‘exclusive-OR’ in terms of  or/and/not/and? 
                           Of course, you may use whatever is relevant from the CLASS 18 slides. 
 
4.  Define a subset S of  Z2 = Z x Z  (=the set of all pairs of negative, zero, positive integers) by the 
          following rules: 
 
     (a)    (3,2)    S 
(b)    if  (x,y)    S, then  (3x – 2y,  x)    S 
 
  Prove, by structural induction, that every element of S looks in fact like  ( 2n+1  + 1,  2n + 1 ). 
 
 
 
 
 
  In my CLASS 20 slides, a binary tree type is defined by the variant 
                        type  'a   btree    =    Empty    |    Node  of    'a   *    'a btree   *   'a btree  
 
 (with related OCaml code; refer to that code), and a number of formulas are claimed to hold true,  
        including   the following 
                             rev ( inorder ( reflect x ) )  =  inorder  x    (* rev for lists *) 
                            postorder ( reflect  x )  =  rev ( preorder  x ) 
  
    
      
 5.  Prove, by structural induction, that indeed the shown code, in CLASS 20 slides, implies 
                         rev ( inorder ( reflect x ) )  =  inorder  x    (* rev for lists *) 
           
 
 
6.  Prove, by structural induction, that indeed the shown code implies 
                        postorder ( reflect  x )  =  rev ( preorder  x ) 
