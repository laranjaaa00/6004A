# 6004A/**
 * You can edit, run, and share this code.
 * play.kotlinlang.org
 */
fun main() {
    println("Hello, world!!!")
// Variaveis 
//
// var - mutável - seu valor pode ser alterado
// val - não multavel - não é possivel alerar seu valor
//
// Tipos de variaveis 
//
// Boolean - verdadeiro ou falso
// String - qualquer texto de qualquer tamanho dentro de ""
// Char - APENAS UM caractere dentro de ''  -->  ex: 6 
// Int - Números inteiros  --> ex: 6
// Double - Números decimais (de forma arredondada)  --> ex: 71.23
// Long - Númerero reais (de forma longa) --> Ex: 5000000000000000000
// Float - Número decimais (deforma definitiva) --> ex: 71.23141626466868
//
// Estrutura de uma variavel 
//
// var nomeDela = "Valor"
// var nomeDela: String

//Concatenação
var messiGoldenBall = 7    
    
println("O Messi já ganhou " + messiGoldenBall + " vezes a bola de Ouro. Ankara Messi")    
println("O messi já ganho $messiGoldenBall vezes a Bola de Ouro. Ankara Messi")    
    
}



///88##########################################



fun main() {
   
    var usuario = ContaBanco(-100.0, 1456156754784564156, 5018)
 usuario.consultarSaldo(5018)
 usuario.deposito(5018, 2.0)
 usuario.consultarSaldo(5018)
 usuario.saque(5018, 20.0)
}





 class ContaBanco(var saldo: Double, var numeroConta: Long, var senhaCorreta: Int){

   fun consultarSaldo(senha: Int){ 
    
    
    
   if(senha == senhaCorreta){
        println("Saldo: R$saldo")
    }else{ 
        println("Senha incorreta")
         }
   }

   fun deposito(senha: Int, valor: Double){
       
       if(senha == senhaCorreta){
          if(valor <= 0){
              println("depósito de R$$valor impossivel de ser realizado")
          }else{ 
              saldo += valor
           println("depósito de R$$valor realizadocom sucesso")
          
          }
         
          
    }else{ 
        println("Senha incorreta")
       
    
       }
   
   }
  
 
 
 //exercício -> Faça o método de sacar na conta do banco
 //
 //

fun saque(senha: Int, valor: Double){

 if(senha == senhaCorreta){
          if(valor <= 0){
              println("saque de R$$valor impossivel de ser realizado")
          }else if(valor > saldo){
              println("saque de R$$valor realizado com sucesso ☺")
               }else{ 
              saldo -= valor
           println("depósito de R$$valor realizadocom sucesso")
          
          }
         
          
    }else{ 
        println("Senha incorreta")
       
    
       }


}
 }








