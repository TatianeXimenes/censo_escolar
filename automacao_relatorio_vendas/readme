# Sistema de Automação de Relatórios de Vendas
Este projeto automatiza a geração e envio de relatórios de vendas por e-mail, com base em uma planilha de vendas. Ele calcula métricas importantes como faturamento, quantidade vendida e ticket médio para cada loja, e envia relatórios personalizados por e-mail.

## 🎯 Objetivo
Automatizar a análise de vendas e o envio de relatórios para a diretoria e para cada loja, facilitando a tomada de decisão e o acompanhamento do desempenho.

## ⚙️ Funcionalidades
- Cálculo do faturamento por loja
- Cálculo da quantidade de produtos vendidos por loja
- Cálculo do ticket médio (faturamento / quantidade)
- Envio de e-mail com relatório consolidado para a diretoria
- Envio de e-mail personalizado para cada loja com seu desempenho

## 🛠️ Tecnologias utilizadas
- Python 3
- Pandas (manipulação de dados)
- smtplib + email (envio de e-mails)

## 🚀 Como executar
- Instale as dependências:

bash
pip install pandas openpyxl

- Coloque o arquivo Vendas.xlsx no mesmo diretório ou ajuste o caminho no código.
- Configure o e-mail remetente e senha no código (veja os ajustes necessários abaixo).

- Execute:

bash
python projeto1.py

## ⚠️ Pontos de atenção / Ajustes necessários
1. Autenticação do e-mail
O código usa login com senha direta, o que não é mais suportado pelo Gmail sem configuração adicional. Recomenda-se:

Usar Senha de App do Gmail (recomendado)
Ou configurar OAuth2 (mais seguro)

2. Erro no cálculo do ticket médio por loja
Na última seção, há um erro de digitação:

python
tabela_loja["Ticker Medio"] = ...  # Errado: "Ticker Medio"
# Deveria ser:
tabela_loja["Ticket Médio"] = ...

3. Segurança da senha
A senha está exposta no código. Em produção, use variáveis de ambiente ou arquivos de configuração seguros.
4. Tratamento de exceções
O código não trata erros de conexão, autenticação ou arquivo não encontrado. Recomenda-se adicionar try/except.
5. Formatação do e-mail
O HTML é simples. Pode ser melhorado com CSS para melhor visualização.

## 📊 Métricas calculadas
Faturamento: Soma do Valor Final por loja
Quantidade: Soma da Quantidade por loja
Ticket Médio: Faturamento / Quantidade

## 📬 Fluxo de envio de e-mails
- Envia relatório consolidado (todas as lojas) para a diretoria
- Envia relatório individual para cada loja

## 🔧 Possíveis melhorias futuras
- Adicionar gráficos (matplotlib/seaborn) nos e-mails
- Suporte a outros provedores de e-mail (Outlook, SMTP próprio)
- Agendamento automático (cron, schedule)
- Salvar relatórios em PDF/Excel antes de enviar
- Dashboard web com Streamlit ou Flask

## 👤 Tatiane Ximenes
Projeto desenvolvido para fins de aprendizado em automação com Python.
