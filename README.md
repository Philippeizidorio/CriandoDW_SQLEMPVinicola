# Criando Um Data Warehouse(DW) No SQL Server Do Setor Comercial De Uma Empresa Produtora De Vinhos 💱🍇
![Alt ou título da imagem](https://github.com/Philippeizidorio/CriandoDW_SQLEMPVinicola/blob/main/wineryfinan.png)

### ◾Contexto:
Ingressando em uma Vinícola de médio porte ___(Empresa Produtora De vinhos)___, depois de um certo tempo, percebi que o ambiente transacional comercial, o qual é alimentado tanto por milhares de dados de vendas do website quanto por funcionários diariamente usando um sistema próprio da empresa, começou a passar por gargalos substanciais devido ao fato do banco de dados (SGBD), neste caso o __SQL Server__, está diretamente conectado a algumas ferramentas de Dataviz que o time de analistas utiliza para criar consultas e acompanhar métricas importantes do setor em tempo real. Dessa forma, para solucionar tal problema, decidi que será necessário implementar um __Online Analytical Processing(OLAP)__ que consiste num repositório separado do ambiente principal, com o objetivo de evitar o sobrecarregamento de ambas as partes, adequando-o conforme os requisitos de negócio e de dados. 

### ◾Requisitos Para Implementação do Data Warehouse:
- Dados serão armazenados localmente;
- Ferramenta Pentaho fará o processo de ETL;
- Deverá ser aplicada uma modelagem multidimensional;
- Deve-se permanecer apenas com as SKs referentes na Fato;
- Realizar remoção de redundâncias nos atributos.

### ◾Steps Utilizados na criação das ___'Dim_Tables'___ Por Meio Da Ferramenta __Pentaho__:
Após definição do projeto e ter trabalhado na arquitetura do nosso DW, é momento de partimos para a conexão e criação das primeiras regras de ETL e através da ferramenta __Pentaho__
com o nosso banco de dados, nesta primeira etapa de transformação, criaremos as _tabelas dimensões_ e aplicaremos todos os steps necessários conforme ilustrado logo a seguir ↓

![DIM](https://github.com/Philippeizidorio/CriandoDW_SQLEMPVinicola/blob/main/ETL%20-%20DIM_Tables.png)

### ◾Steps Utilizados na criação da ___'Fact_Table'___ Por Meio Da Ferramenta __Pentaho__:

![FACT](https://github.com/Philippeizidorio/CriandoDW_SQLEMPVinicola/blob/main/ETL-%20Fact_Table.png)

### ◾Definindo Updates: 
Tendo realizado a primeira carga para validação das etapas anteriores, agora é momento de agendarmos atualizações por meio de uma tarefa ou _'JOB'_ dentro do __Pentaho__. Para isso, devemos levar em consideração as necessidades do negócio bem como o volume e quantidade de dados que serão processados. Neste caso, defini uma atualização para cada 3 minutos, além disso, adicionei uma etapa de notificação por email para sabermos o andamento da situação das atualização.

![jobupdate](https://github.com/Philippeizidorio/CriandoDW_SQLEMPVinicola/blob/main/Update_JOB.png)

### ◾Diagrama Entidade-Relacionamento(DER) Do DW No SQL Server: 

![DER](https://github.com/Philippeizidorio/CriandoDW_SQLEMPVinicola/blob/main/DER_COM_DW.png)

### ◾ Tecnologias Utilizadas: 
<div <br> 
<img src="https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white">
<img src="https://github.com/Philippeizidorio/CriandoDW_SQLEMPVinicola/assets/145637595/a2ff1f77-cccf-45f6-8ecc-5a9735f2e64c">
<img src="https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white">
</div> 

## Autor:

<img  src="https://github.com/Philippeizidorio/Dashboard_PowerBIMarketing/assets/145637595/dd3c301c-3cd3-4808-92c8-a321553f7acf" width="80" alt="cognitiveclass.ai logo" align="left" /> 

### &nbsp;&nbsp;Philippe Izidório

<p>
&nbsp;&nbsp;Cientista de Dados / Business Intelligence / Analista de Dados<br/>
&nbsp;&nbsp;LinkedIn: https://www.linkedin.com/in/philippeizidorio/<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;E-mail: euphilippeizidorio@gmail.com<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Portifólio de projetos em Data Science: https://github.com/Philippeizidorio
</p>

