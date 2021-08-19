#include<iostream>
int main()
{
  std::cout << "==============================\n";
  std::cout << "The Turtle and Rabbit Race - GAME START\n";
  std::cout << "===============================\n";
  std::cout << "Chooose Your Character\n";

 std::cout << "===========================\n";
 std::cout << "1) Turtle\n2) Rabbit\n";
 std::cout << "====================\nEnter the index\n";
 
 int character_index = 0;
 while((character_index > 2) || (character_index == 0)){
 
 std::cin >> character_index;

  std::cout << "===========================\n";
if(character_index == 1)
{
std::cout << "You Choose Turtle\n";
}
else if(character_index == 2){
  std::cout << "You Choose Rabbit\n";
}
else{
  std::cout << "You Choose Unknown Character please reenter the character\n";
}
}
 
}
