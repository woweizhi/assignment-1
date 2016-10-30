# assignment-1
Q1. Linear Recursion only needs to call itself once, and Binary Recursion needs to call itself twice. 
  example Linear Recursion: Factorial 
  Binary Recursion: Fibonacci
  
Q2. non-recursive version of the Factorial Algorithm1
  function Factorial(n)
  Input: non-negative integer n 
  Output:Factorial(n)
  if n == 0 then 
  return 1 
  else 
  while 1 to n 
  int sum <-- 1
  sum = sum*n
  return sum
  end function
  
 Q3.Algorithm 2
Function MatrixArraySum(A,r,c)      
input :non-negative integer  r,c the number of column.
If r==1 than
Return ArraySum(A[0],c)
Else
Return MatrixArraySum(A,r-2,c)+ArraySum(A[r-1],c)
End if

Q4. 1, 1
    2, 10
    4,100
    10,1010
    32,100000
 function: convert decimalism into binary 
 
 Q5. (4,2)  false
     (7,2)  ture 
     (8,2)  false 
     (19,2)  true
     (23,2)  true
function:identify if the number is prime or not 

Q6.  ReverseArray(A,1,5) 
   A = [8,14,6,15,11,3,0,2,3,6]
   when 1<5 reverse A[1] A[5]
   when 2<4 reverse A[2] A[4]
   when 3<2  
   end function 
   so the new array should be A=[8,3,11,15,6,14,0,2,3,6] 
   
Q7.(a) Pseudocode:
  Algorithm GetNode(n,count,curr)
  Input:the nth of node is to be gotten, count indicates how many node we already go through, curr indicates the current node. 
  Output: get the nth node
  void GetNode(n,count,curr)
  GetNode(n,1,head) 
  if (n < LinkedList.size( )) then
  if  count == n then 
  return curr
  else
  return GetNode(n,count+1,curr->next)
(b)Code
void Start() const {
cout<< "Input the n (the nth Node you want to find)" << endl;
cin>>n
return getnth (n,1,head);
}

Node* LinkedList::getnth(int n, int count, Node* curr){
   if (n>this->_size)
       cout<<"There is no nth Node in the LinkedList"<<endl;
   if (count==n) return curr;
   else 
       return getnth(n,count++,curr->set_next(curr->get_next))
}

Q8.
 (a)string reverseString(const string& word) {
	if (word.length()==0||word.length()==1){
		return word;
	}
	else{
		string newWord=word.substr(1,word.length()-2);
		return (word[word.length()-1]+reverseString(newWord)+word[0]);

	}
}
(b) 
bool isPalindrome(const string& word){
int l=word.length();
for(int i=0;i<l/2;i++){
if (word[i] != word[l-i-1] ){
 return false ;
else 
return true;
      }
   }
}
