![cover](.github/cover.png?style=flat)

## 💻 Projeto
Plataforma de eventos criado a partir do evento Ignite Lab da [Rocketseat](https://www.rocketseat.com.br/). O projeto consiste na elaboração de uma landpage e também de uma plataforma de eventos com vídeos podendo conter vídeos aulas, palestras e afins, sendo esses vídeos ao vivo ou não, com data para liberação da exibição, enfim, uma plataforma de eventos completa.

## ✨ Tecnologias

- [React JS](https://pt-br.reactjs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Tailwindcss](https://tailwindcss.com/)
- [GraphCMS](https://app.graphcms.com/)
- [GraphQL](https://graphql.org/)
- [GraphQl-Code-Generator](https://www.graphql-code-generator.com/)

## Executando o projeto

Caso queira executar o projeto por conta a partir desse projeto, então será necessário primeiro você criar uma conta no site do [GraphCMS](https://app.graphcms.com/), caso ainda não tenha claro. E deixarei disponibilizado esse [link](https://app.graphcms.com/clone/b66fea2716c840b58557b5625cc2a0e0?name=Ignite%20Lab%20-%20Event%20Platform) para que você possa fazer a cópia da estrutura do meu projeto no GraphCMS.

Após isso, precisará inserir variáveis ambiente em um arquivo que você precisará criar na raíz do projeto chamado **.env.local**, essas variáveis demonstradas abaixo:
```cl
VITE_API_URL={your_content_api}
VITE_API_ACCESS_TOKEN={your_permanent_auth_token}
```

Para a VITE_API_ACCESS_TOKEN, você precisará criar um token permanente de autenticação com as permissões no **Content API**, permissão de **Read** para todos os models, e mais 2 permissões, permissão de **Read** para **Subscriber** on stage **Draft** e permissão de **Create** para **Subscriber**, feito isso, copiar o token e inserir no arquivo **.env.local** que você criou anteriormente.

Agora com as URLs das variáveis ambientes em mãos, copie a mesma que você colocou em **VITE_API_URL**, vá até o arquivo **codegen.yml** e adicione essa sua URL no lugar da qual esta atualmente em **schema**

Utilize o **yarn** ou **npm install** para instalar as dependências do projeto.

Antes de iniciar o projeto, rode em seu terminal o comando a seguir, para gerar novamente o typescript das queries e mutations do graphql de acordo com seu projeto, talvez não precise, pois caso tenha feito o clone do meu projeto, provavelmente já estará com todo o typescript correto, mas enfim, caso não esteja, você pode estar rodando novamente sem problemas nenhum.
```cl
yarn codegen
ou
npm run codegen
```

Em seguida, inicie o projeto.<br/>

```cl
yarn dev
ou
npm run dev
```

**Observação**: Com a cópia da estrutura do meu projeto em sua conta GraphCMS, junto ao seu token inserido corretamente em um arquivo **.env.local**, o projeto deverá estar funcionando normalmente.


## 📄 Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

---

Feito por Rafael Quartaroli por meio do evento da [Rocketseat](https://www.rocketseat.com.br/).

<br />
