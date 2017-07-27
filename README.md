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

3)3)
take 5 [1..] {- INSERT this in the winghci-}

3)4) 
hello = do
   putStrLn "what is your lottery numbers?"
   name <- getLine
   putStrLn $ "your numbers are " ++ name
 randList <- forM [1 .. lLength] $ \_i -> randomRIO (1,50)
