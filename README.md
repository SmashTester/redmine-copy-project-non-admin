# redmine-copy-project-non-admin
Redmine - Permitir que usuários não administradores copiem determinados projetos


Atualmente, apenas os administradores podem copiar projetos no Redmine, o que não é bom, porque os "Gerentes de Projeto" devem ser capazes de criar, editar e copiar projetos, mas não ter acesso total a todo o restante do Redmine. E a cópia é importante, porque certos projetos são usados como modelos e são apenas copiados  para acelerar o Fluxo.

Pensando nissso foi criado um Patch na aplicação. Esse patch essencialmente verifica se o usuário pode editar o projeto e, em caso afirmativo, concede acesso à cópia. O patch também adiciona um botão para copiar o projeto na área de links contextuais ao visualizar o projeto, claro, somente se o usuário atual puder editá-lo.

Quando algum usuário precisar ter a permissão para copiar projetos ele só precisa solicitar a algum dos administradores do Redmine para colocá-lo em um Grupo que tenha permissão de edição de projetos, como por exemplo as funções de: "Gerentes de Projeto" e "Coordenador".
