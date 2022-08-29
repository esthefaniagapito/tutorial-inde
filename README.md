<img src="https://inde.gov.br/](https://inde.gov.br/img/INDE%20Logo_2.png" heigth="" width="" title="Logo_INDE">
<img src="https://inde.gov.br/](https://inde.gov.br/img/INDE%20Logo_2.png" heigth="" width="" title="Logo_IBGE">

# Guia do Usuário Simplificado INDE
Este guia tem como objetivo esclarecer de uma maneira geral e simplificada as etapas, para a inclusão de recursos geoespaciais ao catálogo de metadados da INDE. O IBGE, como Gestor do DBGD, realiza periodicamente a capacitação da Infraestrutura de Dados Espaciais, para consultar a agenda clique [aqui](https://treinamento.inde.gov.br/).

🚩A distribuição deste material é realizada de forma integralmente gratuita, sendo proibida qualquer forma de uso comercial do mesmo.

## O que é uma Infraestrutura de Dados Espaciais (IDE)?
Um conjunto integrador de tecnologias, padrões, políticas, arranjos institucionais e recursos humanos, necessários, para facilitar a disponibilização, o acesso e o uso de dados e informações geoespaciais.

## Por que existem as IDE's?
- Facilitar a busca, o acesso e a integração de diferentes tipos de geoinformação.
- Integração de base de dados geoespaciais.

## Como funciona uma IDE?
Uma IDE deve permitir aos seus usuários buscas através do navegador, para encontrar, visualizar, usar e combinar informação geoespacial de diferentes produtores de dados, para atender suas necessidades.

## INDE: a IDE brasileira
Infraestrutura Nacional de Dados Espaciais - INDE: conjunto integrado de tecnologias; políticas; mecanismos e procedimentos de coordenação e monitoramento; padrões e acordos, necessário para facilitar e ordenar a geração, o armazenamento, o acesso, o compartilhamento, a disseminação e o uso dos dados geoespaciais de origem federal, estadual, distrital e municipal. 

Contém:
- Diretório Brasileiro de Dados Geoespaciais (DBDG): sistema de servidores de dados distribuídos na internet, com o propósito de reunir os produtores de GI, administradores e usuários, para armazenamento, compartilhamento e acesso a dados geoespaciais e serviços relacionados.
- Geosserviços: WMS, WFS, ECS, SLD, CSW e etc.
- Catálogo de metadados.
- Visualizador VINDE.

## Como aderir à INDE

Para solicitar sua adesão à INDE siga as instruções clicando [aqui](https://inde.gov.br/ComoFazerParte).

## Passo a passo para o registro de metadados
1. Faça o login como administrador no sistema;
2. Crie um grupo.
3. Ainda dentro do perfil de administrador inclua a equipe responsável (revisor, editor e etc).
4. Vá em contribuir > quadro de edição > adicionar novo registro.
5. Realize o preenchimento dos campos necessários.
  5.1 Caso necessite de outros campos que não estejam visíveis, no canto direito superior troque o template padrão para completo.
  5.2 Adicione os elementos que necessite.
6. Clique em Gravar e Fechar.
7. Para publicar vá para contribuir > selecione o recurso a ser publicado > clique em publicar

As etapas seguintes devem ser utilizadas, para produtos digitais.

9. Efetue login no sistema de cargas de dados da INDE.
10. Clique em enviar arquivos > selecione os arquivos > clique em enviar.
11. Ainda no sistema de cargas: banco e esquemas > selecionar o que foi adicionado > iniciar importação

Agora dentro do Geoserver:

12. Efetue login.
13. No menu clique em layer > nova camada > selecione sua base de dados
14. No campo de pesquisa busque digite o nome do recurso a ser vinculado > publish
15. Irá abrir uma nova aba, edite os campos disponíveis. Dica: utilize os próprios metadados inseridos na INDE.
16. Em metadata link clique no botão add link > cole a seguinte url https://inde.gov.br/geonetwork/srv/por/csw?service=CSW&version=2.0.2&request=GetRecordById&id=SEU_CÓDIGO_ID&elementSetName=full&outputSchema=csw:IsoRecord . Lembre-se de editar adicionando o número de identificador gerado pela INDE.
17. Salvar.

Retorne ao catálogo de metadados. 

18. Selecione o recurso que está sendo vinculado o geosserviço > Clique em editar.
19. Vamos adicionar o serviço de WMS: no lado direito > adicionar recurso online > aplicativo usando recurso > url cole o link WMS fornecido pelo Geoserver (use a última versão.
20. Edite o nome e descrição.
21. Salve.
23. Siga o mesmo caminho acima para adicionar o serviço WFS, apenas troque a url pela url de WFS.

Adicionando uma thumbnail.

24. Ainda no lado direito clique em adicionar > vincular um 'visão geral de todo recurso ou subconjunto'.
25. Retorne ao Geoserver > layer preview > busque o recurso > all format > selecione PNG > copie o link.
26. Retorne catálogo de metadados e adicione a url.
27. Edite nome e descrição.
28. Salve.
29. Gravar e fechar.

Pronto!

**Contatos**
</br>
Autor: Esthefani Agapito
</br>
E-mail: esthefani.agapito@ibge.gov.br
</br>
Site Oficial: [INDE](https://inde.gov.br/)
</br>
E-mail DBGD: dbdg@inde.gov.br


**Referências**
</br>
http://www.planalto.gov.br/ccivil_03/_ato2007-2010/2008/decreto/d6666.htm
</br>
https://inde.gov.br/Capacitacao
