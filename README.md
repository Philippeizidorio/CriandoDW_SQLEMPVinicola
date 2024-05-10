# Criando Um Data Warehouse(DW) No SQL Server De Um Setor Financeiro - Empresa Produtora De Vinhos 💱🍇
![Alt ou título da imagem](https://github.com/Philippeizidorio/CriandoDW_SQLEMPVinicola/blob/main/wineryfinan.png)

### ◾Contexto:
Ingressando em uma Vinícola ___(Empresa Produtora De vinhos)___ de médio porte, depois de um certo tempo, percebi que o ambiente transacional financeiro, o qual é alimentado tanto por milhares de dados de vendas do website quanto por funcionários diariamente pelo sistema da empresa, começou a passar por certos gargalos devido ao fato do banco de dados (SGBD), neste caso o __SQL Server__, está diretamente conectado a algumas ferramentas de Dataviz que o time de analistas utiliza para criar consultas e acompanhar métricas importantes do setor em tempo real. Dessa forma, para solucionar tal problema, decidi que será necessário implementar um __Online Analytical Processing(OLAP)__ que consiste num repositório separado do ambiente principal, com o objetivo de evitar o sobrecarregamento de ambas as partes, adequando-se aos requisitos de negócio e de dados. 
