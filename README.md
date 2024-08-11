 cpp1-project
 //guess the number
#include<iostream>
#include<cstdlib>
#include<ctime>
int main(){
    std::srand(std::time(0));
    int randomNumber=std::rand()%100+1;
    int userGuess=0;
    std::cout<<"welcome to the number guessing game:"<<std::endl;
    std::cout<<"i have ganerated a numberbetween 1 to 100"<<std::endl;
    std::cout<<"can u guess what it is?"<<std::endl;
    while(userGuess!=randomNumber){
        std::cout<<"enter ur guess";
        std::cin>>userGuess;
        if(userGuess>randomNumber){
            std::cout<<"too high! try again"<<std::endl;

        }else if(userGuess<randomNumber)
        {
            std::cout<<"Too high!try again"<<std::endl;

        }
        else{
            std::cout<<"congratulations!you guess the correct number";
        }
    }
    return 0;

}

