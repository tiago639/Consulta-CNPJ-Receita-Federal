
# 🔍 Consulta de CNPJ na Receita Federal - Power Automate

Este projeto é uma automação criada no **Power Automate (Microsoft Flow)** para realizar consultas de CNPJ na base da Receita Federal utilizando a API pública da ReceitaWS.

## 📁 Estrutura do Projeto

- `manifest.json`: Arquivo principal de configuração do pacote exportado.
- `Microsoft.Flow/flows/.../definition.json`: Define os passos da automação.
- `apisMap.json`: Mapeamento das APIs utilizadas no fluxo.
- `connectionsMap.json`: Referência às conexões configuradas.

## 🚀 Funcionalidades

- Consulta automática de informações de empresas com base no número do CNPJ.
- Integração com APIs públicas para retorno de dados como razão social, atividade econômica, situação cadastral, entre outros.
- Automação exportada no formato `.zip` compatível com o Power Automate.

## 🌐 API Utilizada

Este fluxo utiliza a API pública da ReceitaWS:

- **Endpoint:** `https://receitaws.com.br/v1/cnpj/{cnpj}`
- **Documentação:** [https://www.receitaws.com.br/](https://www.receitaws.com.br/)

### ⚠️ Limitações da API

- A API pública permite **no máximo 3 requisições por minuto por IP**.
- Para usos mais intensivos ou em produção, recomenda-se adquirir a versão paga ou implementar controle de taxa (rate limiting).
- Uso excessivo pode resultar em **bloqueios temporários**.

## 🔧 Como Importar

1. Acesse o [Power Automate](https://flow.microsoft.com).
2. Vá em **Meus Fluxos** > **Importar** > **Importar pacote (.zip)**.
3. Selecione o arquivo `CONSULTA_CNPJ_RECEITA_20250609173627.zip`.
4. Configure as conexões exigidas (ex: HTTP).
5. Clique em **Importar** para finalizar.

## ⚙️ Requisitos

- Conta ativa no Microsoft Power Automate.
- Conectores configurados corretamente (como HTTP e outros, se aplicável).
- Conexão com a internet para acesso à API pública.
- Familiaridade com variáveis e manipulação de fluxos no Power Automate.

## 📌 Observações

- Esta automação é ideal para validação interna de CNPJs, especialmente em processos de cadastro ou compliance.
- Certifique-se de respeitar os termos de uso da API da ReceitaWS.
- A automação pode ser personalizada conforme a necessidade da organização.

---
## 📄 Licença

Este projeto está licenciado sob a **Licença MIT** — veja o arquivo [LICENSE](LICENSE) para mais informações.

---
## 👤 Autor

**Tiago Fonseca** 
