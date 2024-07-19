<template>
  <!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mago Supremo do Universo</title>
  <link rel="stylesheet" href="css/index.css" media="screen" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" integrity="sha384-k6RqeWeci5ZR/Lv4MR0sA0FfDOM5P8zI2DJKarA4khNQFz5aQXZ7Mo7RcV4jVIhK" crossorigin="anonymous">
</head>

<body>
  <i> <h1>Site de cachorro</h1></i>
  <h2>Para ver os melhores cachorros do Brasil</h2>
  <article class="flex-container">
    <article id="img1">
      <img src="@/assets/cachorro1.jpg">
    </article>
    <article id="img2">
      <p>
        <img src="@/assets/cachorro2.jpg" width="250px">
        <img src="@/assets/cachorro3.jpg" width="250px">
      </p>
    </article>
  </article>

  <article class="espaçamento">
    <iframe width="853" height="480" src="https://www.youtube.com/embed/b2GAnB-MDpY?si=DIW8f_QbyeNOaisp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
  </article>

  <!-- Tabela Responsiva -->
  <article class="tabela-container">
    <h2>Tabela de Seres Humanos</h2>
    <div class="table-container">
      <table>
        <thead>
          <tr>
            <th>Nome</th>
            <th>Idade</th>
            <th>Cidade</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td data-label="Nome">João</td>
            <td data-label="Idade">25</td>
            <td data-label="Cidade">São Paulo</td>
          </tr>
          <tr>
            <td data-label="Nome">Maria</td>
            <td data-label="Idade">30</td>
            <td data-label="Cidade">Rio de Janeiro</td>
          </tr>
          <tr>
            <td data-label="Nome">Pedro</td>
            <td data-label="Idade">22</td>
            <td data-label="Cidade">Curitiba</td>
          </tr>
        </tbody>
      </table>
    </div>
  </article>
</body>

</html>
</template>

<script>
export default {
  name: 'HelloWorld',
};
</script>

<style>
/* Estilos básicos */

.flex-container {
  text-align: center;
}

h1 {
  text-align: center;
  font-size: 30px;
}

h2 {
  text-align: center;
}

#img1 img {
  width: 500px;
  height: auto;
  border-radius: 10px;
  transition: transform 0.3s, box-shadow 0.3s;
}

#img2 {
  display: flex;
  align-content: center;
  justify-content: center;
  align-items: center;
}

#img2 img {
  width: 250px;
  height: auto;
  border-radius: 10px;
  transition: transform 0.3s, box-shadow 0.3s;
}

img {
  border-radius: 10px;
}

iframe {
  width: 600px;
  height: 300px;
  border: none;
  border-radius: 10px;
}

.espaçamento {
  text-align: center;
}

/* Estilos da tabela responsiva */
.table-container {
  width: 90%;
  overflow-x: auto;
  margin: 20px auto;
}

table {
  width: 100%;
  border-collapse: collapse;
  background-color: #fff;
  border: 1px solid #ddd;
}

th, td {
  padding: 12px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}

th {
  background-color: #f2f2f2;
}

@media (max-width: 600px) {
  th, td {
    display: block;
    width: 100%;
    box-sizing: border-box;
  }
  th {
    position: absolute;
    top: -9999px;
    left: -9999px;
  }
  td {
    border: none;
    position: relative;
    padding-left: 50%;
    text-align: right;
  }
  td:before {
    content: attr(data-label);
    position: absolute;
    left: 0;
    width: 50%;
    padding-left: 10px;
    font-weight: bold;
    text-align: left;
    white-space: nowrap;
  }
}

/* Efeitos de hover */

#img1 img:hover,
#img2 img:hover {
  transform: scale(1.05); /* Aumenta um pouco o tamanho */
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); /* Adiciona uma sombra suave */
}

@media (max-width: 563px) {
  #img1 img {
    width: 500px;
  }

  #img2 img {
    width: 250px;
  }

  h1 {
    font-size: 25px;
  }

  iframe {
    width: 500px;
  }
}

@media (max-width: 519px) {
  #img1 img {
    width: 300px;
  }

  #img2 img {
    width: 300px;
  }

  iframe {
    width: 300px;
  }
}
</style>
