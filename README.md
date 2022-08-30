<img src="https://inde.gov.br/](https://inde.gov.br/img/INDE%20Logo_2.png" heigth="150px" width="250px" title="Logo_INDE">
<img src="https://inde.gov.br/](https://inde.gov.br/img/INDE%20Logo_2.png" heigth="150px" width="250px" title="Logo_IBGE">

# Guia do Usuário Simplificado para INDE
Este guia tem como objetivo esclarecer de uma maneira geral e simplificada as etapas, para a inclusão de recursos geoespaciais ao catálogo de metadados da INDE. O IBGE, como Gestor do DBGD, realiza periodicamente a capacitação da Infraestrutura de Dados Espaciais. Consulte a agenda clique [aqui](https://treinamento.inde.gov.br/).

🚩A distribuição deste material é realizada de forma integralmente gratuita, deve ser utilizado para fins de treinamento, sendo proibida qualquer forma de uso comercial do mesmo.

<details open>
<summary>O que é uma Infraestrutura de Dados Espaciais (IDE)?</summary>
<br>
Um conjunto integrador de tecnologias, padrões, políticas, arranjos institucionais e recursos humanos, necessários, para facilitar a disponibilização, o acesso e o uso de dados e informações geoespaciais.
</details>

<details open>
<summary>Por que existem as IDE's?</summary>
<br>
- Facilitar a busca, o acesso e a integração de diferentes tipos de geoinformação.
<br>
- Integração de base de dados geoespaciais.
</details>

<details open>
<summary>Como funciona uma IDE?</summary>
<br>
Uma IDE deve permitir aos seus usuários buscas através do navegador, para encontrar, visualizar, usar e combinar informação geoespacial de diferentes produtores de dados, para atender suas necessidades.
</details>

<details open>
<summary>INDE: a IDE brasileira</summary>
<br>
Infraestrutura Nacional de Dados Espaciais - INDE: conjunto integrado de tecnologias; políticas; mecanismos e procedimentos de coordenação e monitoramento; padrões e acordos, necessário para facilitar e ordenar a geração, o armazenamento, o acesso, o compartilhamento, a disseminação e o uso dos dados geoespaciais de origem federal, estadual, distrital e municipal. 
</details>


## Passo a Passo para o Publicação de Metadados na INDE

### Etapa 01: Registro do Recurso e seus Metadados na INDE

Antes de iniciar esta etapa o usuário precisa estar registrado, podendo ser realizado pelo administrador, editor ou revisor do mesmo grupo. A inclusão de metadados pode ser realizado pelo ``Editor``, no entanto, a publicação só pode ser autorizado por administradores e revisores.

1. Efetue ``login`` no [catálogo de metadado da INDE](https://treinamento.inde.gov.br/geonetwork/) ;
2. Na barra de menu vá para ``contribuir`` > ``adicionar novo registro`` > criar um ``conjunto de dados`` > selecione ``template para recurso MGB 2.0`` > selecione o ``grupo da organização`` > clique em ``criar``.
3. Será aberta uma página para inserir os metadados do recurso (modelo padrão). 
4. Caso necessite inserir outros valores que não aparecem no modelo padrão extenda para o modelo completo: ``dentro da mesma página`` > ``menu superior`` > ``ícone de visualização`` 👀 > selecione ``completo``.
5. Realize o ``preenchimento dos campos`` > clique em ``gravar e salvar``.
7. Para publicar retorne ao menu principal: ``contribuir`` > ``quadro de edição`` > ``selecione o recurso`` > ``publicar``.

Neste momento os metadados do seu recurso já estão disponíveis no catálogo de metadados da INDE. Prossiga para a ``etapa 02``, caso seu recurso seja um recurso digital.

### Etapa 02: Efetuando Carga no Sistema de Cargas de Dados

1. Efetue login no [Sistema de Cargas de Dados da INDE](https://treinamento.inde.gov.br/shpinde/).
2. Clique em ``enviar arquivos`` > ``selecione os arquivos`` > ``enviar``.
3. Ainda no sistema de cargas vá para: ``banco e esquemas`` > ``selecione o que foi adicionado`` > clique em ``iniciar importação``. 


### Etapa 03: Configurando o Geosserviço

1. Efetue login no [GeoServer](https://treinamento.inde.gov.br/geoserver/web/).
2. No menu lateral clique em ``layer`` > ``new layer`` > ``selecione sua base de dados da etapa anterior``.
3. Na barra de pesquisa ``digite o nome do recurso`` > clique em ``publish``.
4. Irá abrir uma nova página semelhante ao formulário de catálogo de metadados da INDE. Edite os campos disponíveis. Dica: utilize os próprios metadados inseridos na INDE.
5. Ainda na mesma página role até ``metadata link`` > clique no botão ``add link`` > copie a url a seguir, substituindo ``SEU_CÓDIGO_ID`` pelo ID do recurso, disponível no catálogo de metadados da INDE: ``https://inde.gov.br/geonetwork/srv/por/csw?service=CSW&version=2.0.2&request=GetRecordById&id=SEU_CÓDIGO_ID&elementSetName=full&outputSchema=csw:IsoRecord``. 
6. Clique em ``salvar``.

### Etapa 04: Vinculando o GeoServer aos Metadados

1. Retorne ao [catálogo de metadados da INDE](https://treinamento.inde.gov.br/geonetwork/srv/por/catalog.search#/home). 
2. ``Selecione recurso`` que está sendo vinculado o geosserviço > Clique em ``editar``.
3. Adicione o serviço de WMS: ``lado direito da página`` > clique em ``adicionar recurso online`` > ``aplicativo usando recurso`` >  em ``url`` cole o link WMS fornecido pelo Geoserver (use a última versão). Para obter o link clique [aqui](https://treinamento.inde.gov.br/geoserver/web/)
4. Edite o ``nome`` e ``descrição``.
5. Clique em ``salvar``.
6. Siga o mesmo caminho acima para adicionar o serviço WFS, apenas troque a url pela url de WFS, disponível na mesma página.

### Etapa 05: Adicionando Thumbnail (miniatura)

24. Ainda no lado direito clique em ``adicionar`` > vincular um ``visão geral de todo recurso ou subconjunto'``
25. Retorne ao ``Geoserver`` > ``layer preview`` > busque o ``recurso`` > ``all formats`` > selecione ``PNG`` > copie o ``link``.
26. Retorne catálogo de metadados e ``adicione a url`` no campo indicado.
27. Edite ``nome`` e ``descrição``.
28. Clique em ``salvar``.
29. Clique em ``gravar e fechar``.

Pronto!✅

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

[Capacitação INDE](https://inde.gov.br/Capacitacao)
