# DesafioDeProgramacao

###### Códigos realizados através da linguagem **C++** podendo ser utilizando em qualquer IDE com extensão de **C++**

###### IDE utilizada: Code::Blocks


## Questao 1
```
#include <iostream>

using namespace std;

int main(){
  int n = 0;
  
  //Inserção de dados
  cout << "Insira um valor: ";
  cin >> n;
  
  //Gerando colunas
  for(int i=1; i<=n; i++){
    //Gerando asteríscos na mesma quantidade de colunas
    for(int j=1; j<=i; j++){
      cout << "*";
      //Checando se está na ultima linha
      if(i<n){
        cout << " ";
      }
    }
  cout << endl;
  }
return 0;
}
```
## Questão 2
```
#include <iostream>
#include <string> //Biblioteca para manipular strings

using namespace std;

int main(){
  int tamanho;
  string senha;
  
  //Inserção de dados
  cout << "Insira sua senha: ";
  cin >> senha;
  
  //Descobrindo tamanho da senha
  tamanho = senha.size();
  
  //Condição para apresentação de caracteres mínimos necessários
  if(tamanho<6){
    cout << "Falta: " << 6-tamanho;
  }else{
   cout << "Tudo OK!"; 
   }
return 0;
}
```
## Questão 3
```
#include <iostream>
#include <string> //Biblioteca para manipular strings

using namespace std;

int main(){
  cout << "Entrada" << endl;
  string palavra;
  
  //Inserção de dados
  cout << "Insira uma palavra: ";
  cin >> palavra;
  
  //Declaração de variáveis
  int tam = palavra.size();
  int tam1 = palavra.size()-1;
  int con=0;
  char letra1, letra2;
  
  cout << endl;
  
  cout << "Saída" << endl;
  //Estrutura de comparação
  for(int i=0; i<=tam; i++){
    for(int j=i+1; j<=tam1; j++){
      if(palavra.at(i)==palavra.at(j)){
        con++;
       }
    }
  }
  cout << con+1;
return 0;
}
```
