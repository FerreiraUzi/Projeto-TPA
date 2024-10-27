# <h1 align="center">Técnicas de programação em algoritmos - ETEC 2024 </h1>
 <h3 align="center"> Conceitos e exemplos práticos de algoritmos: </h3>
<p>     Conceitos básicos, estruturas de comando, laços de repetição, vetores, fluxogramas  e etc... </p>

[![My Skills](https://skillicons.dev/icons?i=js,html,css,php,phyton)](https://skillicons.dev)

## <h2> :new_moon: O que são algoritimos? </h2>
<p>
<ul>
 <li>
Algoritmos são sequências de passos que seguimos com a intenção de atingir um objetivo, pode ser desde atravessar uma rua, fazer um bolo ou definir qual critério usar para aprovar ou reprovar um aluno, por exemplo. <br>
  
No desenvolvimento de um algoritmo, é essencial definir com clareza e precisão o conjunto de regras ou instruções que resolverão um problema específico. <br> 

Assim, antes de iniciar a programação, é importante entender o que deve ser feito e planejar o passo a passo, ou seja, criar o algoritmo e verificar se o resultado obtido atende às expectativas. 

<br> Com essa compreensão, podemos então escolher uma linguagem de programação adequada para implementar nossos algoritmos.
 </li>
</ul>
</p>


## <h2> :waxing_crescent_moon:  Comandos básicos: </h2>

  ## <h3> 💫 Variáveis: </h3>

  <ul>
   <li>
    Variáveis são como "caixas" onde você pode guardar informações que podem mudar enquanto o programa está rodando. Cada variável tem um nome que você escolhe, um tipo que diz que tipo de informação ela vai guardar, como números inteiros (inteiro/int) , decimais (float/real) ou textos(cadeia/caracter) e um valor que é o que está dentro da caixa.
    Você pode definir as variáveis antes do início do programa, como:
   

  
  
    inteiro numero=1

   > Ou pedir que o usuário digite um valor com o comando:

    inteiro numero
     escreva("Digite o valor desejado")
     leia(numero)

> Onde: 

  > 💫  Você deve declarar o tipo e nome da variável antes do comando
  
  > 💫  O comando "escreva" mostra a informação contida dentro do parênteses e das aspas, e pode mostrar o informação contida dentro da variável com a "Concatenação"
  
>   💫 Concatenação serve para mostrar o valor de determinada variável para o usuário, utilizando a fecha das aspas e as virgulas para isso, como no exemplo abaixo onde o valor retornado pela concatenação será 25:
 

````
inteiro variavel=25
escreva("O valor contido dentro da variável é: ", variavel, "!")
````

   
  </ul>

  > [!NOTE]
 > Os códigos podem ser usados um dentro dos outros (funciona com qualquer código).

## <h2> :first_quarter_moon: Estruturas de Controle: </h2>
## <h3> 💫 Se e Senão: </h3>

<ul>
 <li>
 Em várias situações, é necessário tomar decisões.

Nos algoritmos, muitas vezes encontramos a necessidade de avaliar condições e ajustar o fluxo de execução do programa, aplicando ações específicas para diferentes situações. Isso é fundamental para assegurar que o resultado final seja o desejado no desenvolvimento de sites ou aplicativos.

Para implementar essa lógica, utilizamos as palavras-chave "se" e "senão". Elas nos permitem verificar uma condição e determinar qual ação deve ser executada com base nessa avaliação.

</li>
</ul>



```
programa {
  funcao inicio() {
    inteiro teste

    escreva ("Esse código vai pedir um valor ao usuário, e o valor "leia" vai armazenar o valor digitado na variável desejada\n")
    leia(teste)


    se(teste<5){
      escreva("Essa parte do código vai ser executada caso a opção dentro das parenteses da função "se" seja verdadeira")
    }

    senao se( teste<7){
      escreva("Essa parte do código vai ser executada caso existam mais de uma opção, sera executado caso a opção dentro dos parenteses do primeiro "se" seja falsa")
    }

    senao{
      escreva("Essa parte do código vai ser executada caso nenhuma das outras opções sejam verdadeiras")
    }

  }
}


```

## <h3> 💫 Escolha Caso: </h3>

<ul>
 <li>
  Esse comando verifica o valor de uma variável e escolhe um bloco de código para executar com base nesse valor. Se o valor não corresponder a nenhuma das opções, normalmente há uma alternativa padrão que pode ser executada.
 </li>
</ul>

```
programa {
  funcao inicio() {
    inteiro teste

    escreva("1- Opção 1 \n")
    escreva("2- Opção 2 \n")
    escreva("3- Opção 3 \n")
    escreva("4- Opção 4 \n")
    leia(teste)

    escolha (teste){
      caso 1: escreva("Aqui vai ser retornada a opção 1")
      pare

       caso 2: escreva("Aqui vai ser retornada a opção 2")
      pare

       caso 3: escreva("Aqui vai ser retornada a opção 3")
      pare

       caso 4: escreva("Aqui vai ser retornada a opção 4")
      pare

      caso contrario: escreva("Aqui vai ser retornada uma opção caso o valor digitado não seja nenhum dos anteriores")
    }
    
  }
}
```

## <h2> 🌔 Laços de repetições: </h2>

<ul>
 <li>
  Laços de repetição, também conhecidos como loops, são estruturas de controle de fluxo que permitem a execução repetida de um bloco de código
 </li>


  💫 Enquanto: Executa enquanto uma opcão for verdadeira, parecido com o "se" mas ele não parará de executar até que a opção se torne falsa, ex:

```
programa {
  funcao inicio() {
    inteiro teste= 10

    enquanto (teste>9){
      escreva("Nesse caso, a frase contida aqui dentro se repetirá infinitamente, pois teste é maior que 9!")
    }
    
  }
}

```


  
  💫 Faça Enquanto: Executa antes de verificar se a opção for verdadeira ou não, depois de executar uma vez ela funcionará como o "Enquanto"

 ```
programa {
  funcao inicio() {

    inteiro teste=5

    faca{
      escreva("Infelizmente, nesse teste, teste não é maior que 9, então, o conteúdo daqui só aparecerá uma vez :<")
    }
    
    enquanto(teste>9)

    escreva("Isso não está correto :<")

  }
}

```


  
  💫 Para: Executa o código quantas vezes escolhido

  ```
programa {
  funcao inicio() {
    inteiro teste=7, contador

    para(contador=0; contador<=teste; contador++ ){
      escreva("O código contido aqui dentro se repetirá 8 vezes, pois teste vale 7 (lembrando que todas as contagens feitas começam contando o 0) e o contador repetirá o código até que alcance teste\n")
    }
    
  }
}

```
</ul>


## <h2>🌕 Vetores: </h2>
Vetores são uma maneira de armazenar várias informações do mesmo tipo em uma única estrutura. Imagine um vetor como uma "lista" ou uma "prateleira" onde você pode guardar vários itens, todos com características semelhantes.

```
programa {
  funcao inicio() {
    inteiro teste[5], contador

  teste[0]= 4
    teste[1]= 5
     teste[2]= 6
      teste[3]= 7
       teste[4]= 8
       

        para(contador=0; contador<=4; contador++) {
          escreva("Teste é igual a: ", teste[contador], "!\n")
        }
    
  }
}
```
> Onde "[]" determina um vetor e o valor contido dentro dele determina a quantidade de vetores

> Onde "teste[contador]" é o número contido dentro do vetor de teste conforme o contador avança.




## <h2> 🌖 Fluxogramas: </h2>

<ul>
 <li>
  Fluxogramas são representações gráficas de processos ou algoritmos, que ajudam a visualizar a sequência de passos necessários para executar uma tarefa específica. Eles utilizam formas geométricas e setas para mostrar a lógica e o fluxo de um processo, tornando mais fácil entender como as informações se movem de uma etapa para outra. 
  
  
 


|    Forma:     |     Informação:                      |
| ------------- | ------------------------------------ |
| Oval          |  Representa o início e o fim;        |
| Retângulo     |  Representa uma ação;                |
| Losângulo     |  Representa uma decisão;             |
| Seta          |  Representa o caminho do fluxograma. |



  <img src="https://api-blog.rdstation.com/wp-content/uploads/2024/08/AD_4nXeVApNmEw4HpXy593moRrmkLHdfu5-S-IdzT8j4kuGo0iBipz89Wno8kUp4Gp9CU8geaC-rRksjfIQVMwRMpCXQs6VmZYGigJfqBktvOOv2oC_t1BTndSlSus0iX8or8zlOKlBGreI7QPXFKog6tseZLzOlkeyfS6HX0sXBv8TKKbgFRmvPw.png" width=40%>
 </li>
</ul>



## <h2> 💫 Fim! 💫 </h2>

Hello World! Muito obrigada por ler meu ReadMe! 🫶 

<img src="https://purina.com.br/sites/default/files/styles/webp/public/2023-05/racao-para-gato-filhote-saiba-como-alimentar-filhote-de-gato.jpg.webp?itok=mz212YP6" width=40%> </img>
