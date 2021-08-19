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
bool check = false; //Iam using check as flag
for(int i = 0; i < 3 && !check;i++)
 {
 std::cin >> character_index;
 std::cout << "===========================\n";

if(character_index == 1)
{
std::cout << "You Choose Turtle\n";
check = true;
}
else if(character_index == 2){
  std::cout << "You Choose Rabbit\n";
  check = true;
  
}
else{
  std::cout << "You Choose Unknown Character please reenter the character\n";
  check = false;//There is no need for this statement
}
 }

std::cout << "===========================\n";

if(character_index == 1){
std::cout << "So Mr. Turtle The Race Between You and Rabbit will be starting in \n";
std::cout << "===========================\n";}
else if(character_index ==2){
  std::cout << "So Mr.Rabbit The Race Between You and the turtle will be starting in\n";
std::cout << "===========================\n";
}
else{
  std::cout << "You have entered too many time...Sorry\n";
  return 0;
}

std::cout << "33333333333333333\n";
std::cout << "===========================\n";

 
std::cout << "2222222222222222222\n";
std::cout << "===========================\n";

std::cout << "11111111111111111111\n";
std::cout << "===========================\n";

std::cout << "GOOOOOOOOOOOOOOOOOOOOOO!\n";
std::cout << "===========================\n";

if(character_index == 1){
  int answer;

  std::cout << "Mr.Turtle started moving slowly and Rabbit is Moving Faster\n";
  std::cout << "===========================\n";


  std::cout << "What will you do? \n1)Will you Give up...and Accept Your Loss\n2)Continue and Persevere\n";
  std::cout << "===========================\n";


  std::cin >> answer;
  check = false;
  for(int i = 0; i<3 && !check; i++){
  if(answer == 1){
    std::cout << "Sorry,but the game ends Here!\n";
    return 0;
  }
  else if(answer == 2){
    std::cout << "Great Job! Neve Give Up!\n";
    check = true;
    std::cout << "===========================\n";
  }
  
 else{
  std::cout << "Sorry There is no Such option Re-enter\n";
    std::cout << "===========================\n";

  check = false;
}
  }
  if(!check){
    std::cout << "You Time is Up You choose options that doesn't exist\nTerminated\n";
      std::cout << "===========================\n";

    return 0;
  }

  std::cout << "Now You saw a River \n";
    std::cout << "===========================\n";

  std::cout << "Rabbit definitely can't cross this River\n";
    std::cout << "===========================\n";
std::cout << "What wll You do?\n1)Swim over to another side2)Help the Rabbit as Rabbit can't swim.\n";
std::cout << "Choose Your Option: ";
std::cin >> answer;
  std::cout << "\n===========================\n";
   
  

  check = false;

  for(int i = 0; i<3 && !check; i++){
  if(answer == 1){
    std::cout << "You Swam to another side.";
    return 0;
  }
  else if(answer == 2){
    std::cout << "You helped the Mr.Rabbit and You both reached the opposite shore\n";
    check = true;
    std::cout << "===========================\n";
  }
 
else{
  std::cout << "Sorry There is no Such option Re-enter\n";
    std::cout << "===========================\n";

  check = false;
}
  }
  if(!check){
    std::cout << "You Time is Up You choose options that doesn't exist\nTerminated\n";
      std::cout << "===========================\n";

    return 0;
  }

  int answer2;

if(answer == 1){
  std::cout << "Now You have Encountered hill with a Steep slope\n You can't move up\n";
  std::cout << "What will You do?1)Go back and ask Mr.Rabbit Help and inturn help him cross the river\n2)Accept Your Defeat and Refuse to take Mr.Rabbits Help.\n";
  
  std::cout << "Enter Your Answer: ";
  std::cin >> answer2;
 check = false;

  for(int i = 0; i<3 && !check; i++){
  if(answer2 == 1){
    std::cout << "Mr.Rabbit decided to Help You\n";
    std::cout << "===========================\n";
    std::cout << "You and Mr.Rabbit Both Won the Race";
    return 0;
  }
  else if(answer2 == 2){
    std::cout << "You should rely on others sometimes to reach your destination\nGAME END\n";
    check = true;
     std::cout << "===========================\n";
    return 0;
  }
 
else{
  std::cout << "Sorry There is no Such option Re-enter\n";
    std::cout << "===========================\n";

  check = false;
}
  }
  if(!check){
    std::cout << "You Time is Up You choose options that doesn't exist\nTerminated\n";
      std::cout << "===========================\n";

    return 0;
  }
}
else if(answer == 2){
  int answer3 = 0;
  std::cout << "What will You do?1)Will You ask the Mr.Rabbits Help?2)Do You Expect the Rabbit to Help?\n";
  std::cout << "Enter Your Answer\n";
  std::cin >> answer3;
  check = false;

  for(int i = 0; i<3 && !check; i++){
  if(answer3 == 1){
    std::cout << "Mr.Rabbit decided to Help You\n";
    std::cout << "=================================================\n";
    std::cout << "You and Mr.Rabbit both Won!\n";
    return 0;
  }
  else if(answer3 == 2){
    std::cout << "You should rely on others sometimes to reach your destination\nGAME END\n";
    std::cout << "Mr.Rabbit won as you never asked his Help\n";
    check = true;
    std::cout << "===========================\n";
    return 0;
  }
  
else{
  std::cout << "Sorry There is no Such option Re-enter\n";
    std::cout << "===========================\n";

  check = false;
}
  }
  if(!check){
    std::cout << "You Time is Up You choose options that doesn't exist\nTerminated\n";
      std::cout << "===========================\n";

    return 0;
  }
}


}
else if(character_index == 2){
  int answer;

  std::cout << "Mr.Turtle started moving slowly and You're Moving Much Faster\n";
  std::cout << "===========================\n";


  std::cout << "What will you do? \n1)Will you Sleep...and Consider Your Win\n2)Continue and Persevere\n";
  std::cout << "===========================\n";


  std::cin >> answer;
  check = false;
  for(int i = 0; i<3 && !check; i++){
  if(answer == 1){
    std::cout << "Tortoise is Moved Very Far and You were Declared to be eliminated from race\n";
    return 0;
  }
  else if(answer == 2){
    std::cout << "Great Job! Neve Give Up!\n";
      std::cout << "===========================\n";
    check = true;
  }

else{
  std::cout << "Sorry There is no Such option Re-enter\n";
    std::cout << "===========================\n";

  check = false;
}
  }
  if(!check){
    std::cout << "You Time is Up You choose options that doesn't exist\nTerminated\n";
      std::cout << "===========================\n";

    return 0;
  }

  std::cout << "Now You saw a River \n";
    std::cout << "===========================\n";

  std::cout << "You definitely can't cross this River\n";
    std::cout << "===========================\n";
std::cout << "What wll You do?\n1)Swim over to another side and Die.2)Ask the Turtle for Help as You can't swim.\n";
std::cout << "Choose Your Option: ";
std::cin >> answer;
  std::cout << "\n===========================\n";
   
  

  check = false;

  for(int i = 0; i<3 && !check; i++){
  if(answer == 1){
    std::cout << "You Died.";
    return 0;
  }
  else if(answer == 2){
    std::cout << "You were helped by the Mr.Turtle and You both reached the opposite shore\n";
    std::cout << "===========================\n";
    check = true;
  }
  
else{
  std::cout << "Sorry There is no Such option Re-enter\n";
    std::cout << "===========================\n";

  check = false;
}
  }
  if(!check){
    std::cout << "You Time is Up You choose options that doesn't exist\nTerminated\n";
      std::cout << "===========================\n";

    return 0;
  }

  int answer2;

if(answer == 2){
  std::cout << "Now You have Encountered hill with a Steep slope\n Turtle can't move up\n";
  std::cout << "What will You do?1)Help the Turtle and Repay his Kindness\n2)You go alone leaving Mr.Turtle.\n";
  
  std::cout << "Enter Your Answer: ";
  std::cin >> answer2;
 check = false;

  for(int i = 0; i<3 && !check; i++){
  if(answer2 == 1){
    std::cout << "You decided to Help You\n";
    std::cout << "===========================\n";
    std::cout << "You and Mr.Turtle Both Won the Race";
    std::cout << "GAME OVER! CONGRATS!";
    return 0;
  }
  else if(answer2 == 2){
    std::cout << "Eventhough You Won the Race ...No one appreciated You and declared Mr.Turtle gave People's Choice Award and You were Ignored\nGAME END\nYOU LOSE";
    std::cout << "===========================\n";
    check = true;
    return 0;
  }
  
else{
  std::cout << "Sorry There is no Such option Re-enter\n";
    std::cout << "===========================\n";

  check = false;
}
  }
  if(!check){
    std::cout << "You Time is Up You choose options that doesn't exist\nTerminated\n";
      std::cout << "===========================\n";

    return 0;
  }
}

}



}



