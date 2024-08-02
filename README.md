# FullStack

## Objetivo
Crie uma aplicação CRUD simples para gerenciar "Tarefas" (Tasks). A aplicação deve permitir a criação, leitura, atualização e exclusão de tarefas. As tarefas devem ter um título, uma descrição e um campo datepicker de deadline.

### Requisitos do Frontend (Angular)

1. **Página Principal**
   - Exiba uma lista de tarefas com opções para editar e excluir.
   - Inclua um Botão para adicionar novas tarefas.
   - Inclua um Input para filtrar as tarefas por nome OU descrição
   - Exiba a contagem dos dias restantes até o deadline para cada tarefa. Se o deadline já tiver passado, exiba uma indicação de problema/erro.

2. **Formulário de Tarefa**
   - Um formulário para criar e editar tarefas. O formulário deve ter campos para o título e a descrição da tarefa e deadline.
   - Valide os campos do formulário (por exemplo, título obrigatório).

### Requisitos do Backend (NestJS)

1. **Modelo de Dados**
   - Crie um modelo de dados para as tarefas usando TypeORM.
   - Crie um banco de dados que utilize o PostgreSQL
   - Crie a(s) tabelas necessárias utilizando migrations do TypeORM (https://typeorm.io/migrations#creating-a-new-migration)
   - Adicione uma coluna virtual no modelo de dados para calcular a contagem dos dias restantes até o deadline.

2. **Endpoints CRUD**
   - **GET** `/task` - Lista todas as tarefas - Deve ser possível filtrar, caso tenha algo na requisição
   - **POST** `/task` - Cria uma nova tarefa.
   - **GET** `/task/:id` - Retorna uma tarefa específica.
   - **PUT** `/task/:id` - Atualiza uma tarefa existente.
   - **DELETE** `/task/:id` - Exclui uma tarefa.

3. **Validação e Erros**
   - Inclua validações básicas para os dados da tarefa. (https://docs.nestjs.com/techniques/validation)
   - Trate erros e forneça respostas apropriadas para operações de CRUD.

4. **Coluna Virtual**
   - Adicione uma coluna virtual que calcule a contagem dos dias restantes até o deadline. Esta coluna deve ser incluída na resposta do endpoint GET `/task`.

### Desafio

**Objetivo:** Integrar o frontend e o backend para permitir a interação completa com o CRUD de tarefas.

1. **Configuração do Ambiente**
   - Configure o projeto Angular e NestJS com TypeORM.
   - Utilize **Tailwind CSS** e/ou **Bootstrap** para estilizar a interface de usuário.

2. **Implementação**
   - Desenvolva as funcionalidades de CRUD no backend.
   - Desenvolva a interface do usuário em Angular e conecte-a aos endpoints do backend.
   - Certifique-se de que o frontend e o backend se comunicam corretamente.

### Instruções para o Candidato

1. **Criação do Repositório**
   - Crie um repositório Git para o projeto e compartilhe o link com a sua implementação.

2. **Documentação**
   - Inclua um README com instruções sobre como configurar e executar o projeto, incluindo qualquer configuração necessária para o banco de dados.

3. **Dúvidas**
   - Caso tenha alguma dúvida ou encontre dificuldades, sinta-se à vontade para perguntar.

### Avaliação

1. Profundidade do conhecimento técnico demonstrado e a capacidade de aplicar soluções criativas e eficazes para os desafios propostos.

2. Habilidade de resolver problemas de forma simples e eficiente, garantindo que as soluções sejam práticas e bem estruturadas.

3. Adesão às boas práticas de codificação, focando na clareza, organização e manutenção adequada do código.

### Envio do teste

- Para enviar o teste, publique o conteúdo no seu repositório pessoal do GitHub. Certifique-se de que o repositório está configurado corretamente e inclui todas as instruções necessárias para a configuração e execução do projeto. Compartilhe o link do repositório quando estiver pronto.

Boa sorte, Imagine Apps.
