<h1 align=center>setTimeout</h1>
<p>
  é uma função nativa do próprio navegador,
  que executa uma função depois de um determinado
  tempo
</p>

<br>
const input = document.querySelector('input[name="price"]')<br>
  input.addEventListener('keydown' , (e)=>{<br>
      setTimeout(()=>{<br>
          let { value } = e.target<br>
          <br>
          value = value.replace(/\D/g , "")
          <br>
          e.target.value = value
          <br>
          console.log(e.target.value)<br>
      } , 1)<br>
  })<br>
  <br>
  
  <p>
    aqui por exemplo , a função não está dexando digitar caracteres,
    por causa do replace... e logo após da executar a função, você
    indica um tempo para executar tudo
  </p>

<strong>Infos adicionais:</strong>
 <br>
 <strong>keydown</strong> = é um dom , que pode pegar tudo que está sendo digitado(no caso no input),
 mas , tem de específicar se você quer o value
 
 EX: e.target.value
<br>
<br>
 <strong>Replace</strong> = só funciona com strings. ela consegue substituir  tudo.
 
 EX:<br>
  <p> g == GLOBAL, PEGA TUDO QUE SE ENCAIXAR<br>
   value.replace(/\sequencia/g , "") == REMOVE TUDO QUE ESTIVER NESSA SEQUENCIA EXATA (EX: SE , QUE)<br>
   value.replace(/\D/g , "") == REMOVE TODOS OS CARACTERES<br>
   value.replace(/\d/g , "") == REMOVE TODOS DIGITOS<br>
   value.replace(/\W/g , "") == REMOVE TODOS OS CARACTERES ESPECIAIS COMO => (. , $)  (W maiusculo)<br>
   value.replace(/\w/g , "") == REMOVE TUDO ,MENOS OS CARACTERES ESPECIAIS (w minusculo)<p/>
=====================================================================================================

