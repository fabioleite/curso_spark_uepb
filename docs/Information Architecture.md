# DIF INFORMATION ARCHITECTURE


O objetivo da arquitetura de informação DIF (_Data Integration Framework_) é coletar dados dispersos dentro e fora de uma
empresa e transformá-los em informações que a empresa usa para operar e planejar o futuro.

Os dados são coletados, transformados usando **regras de negócios** e **conversões técnicas**,
**armazenados em bancos de dados** e **disponibilizados aos usuários de negócios para relatórios e
análises**.

## Fluxo dos dados
> Os dados fluem da criação até a transformação em informação, 
assim como os materiais fluem do fornecedor (sistemas de planejamento de recursos empresariais, sistemas transacionais)
para a fábrica (integração de dados), para armazéns (armazéns de dados - DWs) e, finalmente, para lojas varejistas
(aplicativos de análise de negócios e dados).

A arquitetura de informação DIF ilustrada na Figura apresenta os seguintes componentes:

- Coleta de dados
- Transformação de dados
- Armazenamento de dados
- Disponibilização de informações
- Análise e relatórios

Essa arquitetura visa fornecer uma estrutura integrada para gerenciamento de dados,
permitindo que as empresas tomem decisões informadas com base em informações precisas e
atualizadas.

![Information Architecture](/docs/information_architecture.png)

Observações:

- DIF (Data Integration Framework) é uma estrutura para integração de dados.
- DWs (Data Warehouses) são armazéns de dados centralizados.
- Data marts são armazéns de dados especializados para análise de negócios.
- Business analytics são aplicativos para análise de negócios.