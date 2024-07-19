<template>
<body>
  <i> <h1>Site de cachorro</h1></i>
  <h2>Para ver os melhores cachorros do Brasil</h2>
  <Tabela/>
</body>


    </template>

<script>

import Tabela from "./Tabela.vue";

export default {
  name: 'PaginaPrincipal',
  components: {
    Tabela,
  }
};
</script>

<style>
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
