# Criando Um Data Warehouse(DW) Num Ambiente SQL Server Do Setor Financeiro - Empresa Produtora De Vinhos 💱🍇
![Alt ou título da imagem](https://github.com/Philippeizidorio/CriandoDW_SQLEMPVinicola/blob/main/wineryfinan.png)

### ◾Contexto:
Ingressando numa Vinícola ___(Empresa Produtora De vinhos)___, depois de um certo tempo, percebi que o ambiente transacional financeiro, o qual é alimentado por funcionários diariamente pelo sistema da empresa, está passando por certos gargalos pelo fato do banco de dados (SGBD), neste caso o __SQL Server__, está diretamente conectado à ferramenta de BI que o time de analistas utiliza para acompanhar métricas importantes do setor em questão. Dessa forma, para solucionar isso, decidi que será necessário implementar um __Online Analytical Processing(OLAP)__ que consiste num repositório separado do ambiente principal, com o objetivo de evitar o sobrecarregamento em ambas as partes. 
