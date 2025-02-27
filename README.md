Download link :https://programming.engineering/product/mp5-2-basic-adt-programming-data-structure-creation-pair_sums/

# MP5.2.-Basic-ADT-Programming-Data-Structure-Creation-pair_sums
MRecursive User-Defined Algebraic Data Types pair_sums

The purpose of this question is to help the student master:

Constructing data structures from algebraic data types

Throughout this assignment you may use any library functions you wish.

Problem

Using the type exp found in common.ml and described above, write a term in our language (an abstract syntax tree) that represents the function declaration that implements the following PicoML function pair_sums

let rec pair_sums lst =

if lst = [] then []

else let x = (hd lst) in (fst x + snd x) :: (pair_sums (tl lst))

in pair_sums [(7,1);(4,2);(6,3)]

# let pair_sums = …

val pair_sums : exp =

# string_of_exp pair_sums;;

– : string =

“let rec pair_sums lst = if lst = [] then [] else let x = hd lst

in ((fst x) + (snd x)) :: (pair_sums (tl lst))

in pair_sums (((7,1)) :: (((4,2)) :: (((6,3)) :: [])))”P5.2. Basic ADT Programming, Data Structure Creation, pair_sums
