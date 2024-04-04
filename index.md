#HTML

*Hypertext*
*markup*
*language*

- Tags 

#JavaScript

// variaveis 

const mensagem = "Oi, tudo bem?"

//tipos de dados
  //number
  //string


//funções
alert(mensagem)
const atualizarLista =()=> { //arrow function 


----------------------------------
Código versão 1 JS:
//objeto javaScript
const participante = {
  nome: "Ale Souza",
  email: "ale@gmail.com",
  dataInscricao: new Date(2024, 2, 22, 19, 20),
  dataCheckIn: new Date(2024, 2, 25, 22, 00)
}

//array []
let participantes = [
  {
    nome: "Ale Souza",
    email: "ale@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  }

]

const criarNovoParticipante = (participante) => {
  return `
  <tr>
      <td>
        <strong>
      ${participante.nome}
      </strong>
        <br>
        <small>
        ${participante.nome}
      </small>
    </td>
      <td> ${participante.dataInscricao}</td>
      <td> ${participante.dataCheckIn}</td>
    </tr>

  `
}

const atualizarLista = (participante) => {
  //substituir informação do HTML
  document
    .querySelector('tbody')
    .innerHTML = criarNovoParticipante(participante)

}

atualizarLista(participante)


--------------------------------- Código versão 2 JS

const atualizarLista = (participantes) => {
  let output =""
  // estrutura de repetição loop
  for(let participante of participantes)
  // faça algo aqui enquanto houver participantes na lista
   {
    output = output + criarNovoParticipante(participante)
  }


#CSS
Cascading StyleSheet

table{
  padding: 32px;
  border: 1px solid green;
  margin: 32px;
}

color: #c4c4cc; - cor puxado pro cinza q eu gosto
background-color: #594986; - cor puxado pro roxo/lilás que eu gosto

Meu código : 

body, table, input, button{
  font: 300 16px/140% 'Roboto', sans-serif;
}

body {
background-color: #594986;
color: antiquewhite;
font: 16px 'Roboto', sans-serif;
}

table thead {
  font-size: 14px;
  line-height: 16px ;
}

thead th,
tbody td{
  padding: 12px 16px;
}

tbody td{
  border-top: 1px solid #ffffff1a;
  font-size: 13px;
  line-height: 15px ;
  color: #c4c4cc;
}

tbody td strong {
  color: white;
  font-size: 14px;
  line-height: 16px;
 font-weight: 600;
}

tbody td small {
font-size: 12px;
line-height: 16px;
}

tbody td button {
  all: unset;
  color: #9ff9cc;
}

tbody td button:hover{
  text-decoration: underline;
}

Meu código HTML
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap" rel="stylesheet">


<script src="https://cdn.jsdelivr.net/npm/dayjs@1/dayjs.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/dayjs@1/plugin/relativeTime.js"></script>
<script>
  dayjs.extend(window.dayjs_plugin_relativeTime)
</script>
<script src="https://cdn.jsdelivr.net/npm/dayjs@1/locale/pt-br.js"></script>
<script>
  dayjs.locale('pt-br')
</script>

 <body>

<form onsubmit="adicionarParticipante(event)">
  <fieldset>
    <legend> Inscrição </legend>
    <div>
      <input
  type="text"
  placeholder="Nome Completo"
  name ="nome"
  required
>

      <input
  type="email "
  placeholder="Email"
  name ="email"
  required
>

      <button>
REALIZAR INSCRIÇÃO
</button>

    </div>

  </fieldset>

</form>

<table width="100%">
  <thead style="text-align: left">
    <trd>
      <th>Participante</th>
      <th>Data da inscrição</th>
      <th>Data do check-in</th>

      </tr>
</thead>
<tbody>
</tbody>
</table>

    </body>

  
Meu código JS
let participantes = [
  {
    nome: "Fran ",
    email: "fb@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  },
  {
    nome: "Ana",
    email: "ana@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  },
  {
    nome: "Carlos",
    email: "carlos@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  },
  {
    nome: "Bruna",
    email: "bruna@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  },
  {
    nome: "Daniel",
    email: "daniel@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  },
  {
    nome: "Eduardo",
    email: "eduardo@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  },
  {
    nome: "Fernanda",
    email: "fernanda@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  },
  {
    nome: "Gabriel",
    email: "gabriel@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  },
  {
    nome: "Helena",
    email: "helena@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  },
  {
    nome: "Isabela",
    email: "isabela@gmail.com",
    dataInscricao: new Date(2024, 2, 22, 19, 20),
    dataCheckIn: new Date(2024, 2, 25, 22, 00)
  }
];

const criarNovoParticipante = (participante) => {
  const dataInscricao = dayjs(Date.now())
    .to(participante.dataInscricao)
  let dataCheckIn = dayjs(Date.now())
    .to(participante.dataCheckIn)


  // condicional
  if (participante.dataCheckIn == null) {
    dataCheckIn = `
      <button>  
       data-email="${participante.email}"
       onclick="fazerCheckIn(event)"
       >
      Confirmar check-in
      </button>
       `
  }

  return `
  <tr>
      <td>
        <strong>
      ${participante.nome}
      </strong>
        <br>
        <small>
        ${participante.email}
        </small>
        <small>
        ${participante.nome}
      </small>
    </td>
      <td> ${dataInscricao}</td>
      <td> ${dataCheckIn}</td>
    </tr>
  `
}
const atualizarLista = (participantes) => {
  let output = ""
  for (let participante of participantes) {
    output = output + criarNovoParticipante(participante)
  }
  //substituir informação do HTML
  document
    .querySelector('tbody')
    .innerHTML = output

}
atualizarLista(participantes)

const adicionarParticipante = (event) => {
  event.preventDefault()

  const dadosDoFormulario = new FormData(event.target)

  const participante = {
    nome: dadosDoFormulario.get('nome'),
    email: dadosDoFormulario.get('email'),
    dataInscricao: new Date(),
    dataCheckIn: null
  }
  //verificar se o participante já existe
  const participanteExiste = participantes.find(
    (p) => p.email == participante.email
  )

  if (participanteExiste) {
    alert('Email já cadastrado!')
    return
  }

  participantes = [participante, ...participantes]
  atualizarLista(participantes)

  // limpar o formulário
  event.target.querySelector('[name="nome"]').value = ""

  event.target.querySelector('[name="email"]').value = ""

}

const fazerCheckIn = (event) => {
  //confirmar se realmente quer fazer o check in

  const mensagemConfirmacao = 'Tem certeza que deseja fazer o check-in?'

  if (confirm(mensagemConfirmacao) == false) {
    return
  }
  alert(resultado)
  //encontrar o participante dentro da lista
  const participante = participantes.find((p) => {
    return p.email = event.target.dataset.email
  })
  // atualizar o check in do participante
  participante.dataCheckIn = new Date()

  //atualizar a lista de participantes
  atualizarLista(participantes)
}