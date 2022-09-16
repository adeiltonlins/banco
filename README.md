# banco
function banco(conta, saldo, tipo, agencia, deposito){  
  this.conta = conta;
  this.deposito = deposito;
  this.saldo  = saldo;
  this.tipo = tipo;
  this.agencia = agencia;
  this.SaldoValor =  SaldoValor; 
  this.NumConta = NumConta;
  this.Depositar = Depositar;
  function NumConta(){
    return this.conta;
  }  
   function SaldoValor(){
    return this.saldo;
  }
  function Depositar(deposito){
    this.saldo = saldo + deposito;    
  }      
}


saldo = 20;

conta = prompt("Digite a sua conta: ");
tipo = prompt("Digite seu tipo de conta: ");
deposito = parseInt(prompt("Digite o valor a ser depositado: "));
agencia = prompt("Digite a sua agencia: ");
var minhaConta = new banco(conta, saldo, tipo,  agencia, deposito);
minhaConta.Depositar(deposito);
console.log('O valor após o depósito é: ', minhaConta.SaldoValor());
minhaConta.NumConta();
console.log('A sua conta é: ', minhaConta.NumConta());
