# Criando Um Data Warehouse(DW) No SQL Server Do Setor Comercial De Uma Empresa Produtora De Vinhos 💱🍇
![Alt ou título da imagem](https://github.com/Philippeizidorio/CriandoDW_SQLEMPVinicola/blob/main/wineryfinan.png)

### ◾Contexto:
Ingressando em uma Vinícola de médio porte ___(Empresa Produtora De vinhos)___, depois de um certo tempo, percebi que o ambiente transacional, o qual é alimentado tanto por milhares de dados de vendas do website quanto por funcionários diariamente pelo sistema da empresa, começou a passar por gargalos substanciais devido ao fato do banco de dados (SGBD), neste caso o __SQL Server__, está diretamente conectado a algumas ferramentas de Dataviz que o time de analistas utiliza para criar consultas e acompanhar métricas importantes do setor em tempo real. Dessa forma, para solucionar tal problema, decidi que será necessário implementar um __Online Analytical Processing(OLAP)__ que consiste num repositório separado do ambiente principal, com o objetivo de evitar o sobrecarregamento de ambas as partes, adequando-o conforme os requisitos de negócio e de dados. 

### ◾Requisitos Para Implementação do Data Warehouse:
- Dados serão armazenados localmente;
- Ferramenta Pentaho fará o processo de ETL;
- Deverá ser aplicada uma modelagem multidimensional;
- Criar 4 tabelas Dimensão;
- Criar 1 tabela Fato Associativa;
- Deve-se permanecer apenas com as SKs referentes na Fato;
- Realizar remoção de redundâncias nos atributos.
