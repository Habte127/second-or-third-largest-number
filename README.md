# Second and Third Largest Elements

## Student Information

Name: Habtamu Ayele  
Student Id: RMNS-9485/-23  
Course: Data Structure and Algorithm  

## Algorithm  
1. Input: A vector of integers arr.  
2. Edge Case Handling:  
   - If the array has fewer than 2 unique elements, the second/third largest elements may not exist.  
   - Uses INT_MIN to initialize placeholder values and detect invalid results.  
3. Steps:  
   - Initialize largest, secondLargest, and thirdLargest to INT_MIN.  
   - Traverse the array:  
     - If an element exceeds largest, update thirdLargest → secondLargest → largest.  
     - Else if it exceeds secondLargest and is distinct from largest, update thirdLargest → secondLargest.  
     - Else if it exceeds thirdLargest and is distinct from both higher ranks, update thirdLargest.  
   - Print error messages if secondLargest or thirdLargest remain INT_MIN (no valid elements found).  

## How to Run the Code  
1. Clone the repository to your local machine.  
2. Open the terminal and navigate to the repository directory.  
3. Compile the C++ code:  
   `bash  
   g++ main.cpp -o main
