<template>
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
</template>

<script>
export default {
    name: 'Tabela',
    props: {
        msg: String
    }
};
</script>