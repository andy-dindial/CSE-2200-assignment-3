# CSE-2200-assignment-3
3)1) 

insertAt :: Int -> Int-> [Int] -> [Int] 
insertAt z y xs = as ++ (y:bs)
                  where (as,bs) = splitAt z xs
{-
y is number being inserted 
xs is the list of numbers 
z is the place to be inserted at -}



3)2)

isfib :: Int -> Bool
isfib 1 = False
isfib 2 = True
isfib n   1 : 1: [a + b | (a,b) <- zip fib (tail fib)]
         otherwise = False
isfib300 = fib !! 300



3)3) take 5 [1..]
