***Aluno***   
RF01, RF04, RF05, RF06, RF10  
- idAluno  
- nome  
- cpf
- email    
- telefone  
- endereco  
- rfid  
- status

- contratarPLano()
  agendarAula()
  cancelarAgendamento()
  atualizarStatus()
  registrarAcesso()
  receberNotificacao()

***Plano***  
RF01, RF02, RF04  
- idPlano  
- nome  
- tipo  
- valor  
- ativo

- ativar()
  desativar()
  alterarValor()
  
***Pagamento***  
RF03, RF04, RF09  
- idPagamento   
- data  
- valor  
- formaPagamento  
- status

- registrar()
  confirmar()
  cancelar()

***Acesso***  
RF05, RF09  
- idAcesso  
- dataHora  
- autorizado

- registrar()
    autorizar()
    negar()

***Aula***  
RF06, RF07, RF09  
- idAula  
- nome    
- horario  
- capacidadeMaxima

-    disponibilizarhorario()
    reservarvaga()
    liberarvaga()
    registrarprsenca()

***Agendamento***  
RF06, RF10  
- idAgendamento  
- dataReserva  
- status

-     confirmar()
    cancelar()

***Presenca***  
RF07  
- idPresenca  
- data  
- presente

-     registrar()
    confirmar()

***AvaliacaoFisica***  
RF08, RF10    
- idAvaliacao  
- data  
- peso  
- imc  
- percentualGordura   
- observacoes  
- anexo

-  registrar()
    atualizardados()
    anexararquivo()

***Notificacao***  
RF10  
- idNotificacao  
- tipo  
- dataEnvio  
- status  
- mensagem

- enviar()
    marcarcomolida()
  
***abstract class Funcionario()***

***Instrutor***  
RF07, RF08  
- idInstrutor  
- nome  
- especialidade

- registrarpresenca()
realizaravaliacaofisica()

***Recepcionista***  
RF01, RF03  
- idRecepcionista  
- nome

-  cadastraraluno()
    registrarpagamento()

***Gerente***  
RF02, RF09   
- idGerente  
- nome

-  gerenciarplanos()
    emitirrelatorios()
