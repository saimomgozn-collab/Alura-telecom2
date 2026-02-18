# Alura-telecom2

📊 Previsão de Churn: Estratégias de Retenção na Telecom X
👨‍💻 Sobre Mim
Eu sou o Saimom, CEO Join Visual Tecnologia e graduando em Ciência da Computação e Cibersegurança pelo Gran Centro Universitário. Minha trajetória une a infraestrutura tecnológica à análise de dados, com foco em transformar informações brutas em camadas de defesa e inteligência para o negócio.

🎯 O Desafio
O objetivo deste projeto foi analisar o comportamento de clientes de uma empresa de telecomunicações para prever a evasão (Churn). Mais do que gerar um modelo preditivo, foquei em identificar os gatilhos que levam o cliente a cancelar o serviço, permitindo a criação de estratégias de retenção baseadas em dados.

🛠️ Stack Tecnológica
Linguagem: Python

Bibliotecas de Dados: Pandas, NumPy

Visualização: Seaborn, Matplotlib

Machine Learning: Scikit-learn (Logistic Regression, Random Forest, StandardScalar)

Processamento: SMOTE (Synthetic Minority Over-sampling Technique)

🚀 Meu Pipeline de Desenvolvimento
1. ETL e Tratamento de Integridade
Iniciei normalizando os dados brutos de um JSON. Garanti a integridade da tipagem de variáveis críticas, como o faturamento total, e removi identificadores únicos que não agregavam poder estatístico ao modelo.

2. Engenharia de Atributos e Balanceamento
Identifiquei um desequilíbrio nas classes de evasão (apenas ~26% de Churn). Para evitar que os modelos ficassem enviesados, utilizei o SMOTE para balancear o conjunto de treino, garantindo que o algoritmo aprendesse a identificar padrões de evasão com a mesma precisão que identifica a retenção.

3. Modelagem Preditiva
Optei por comparar dois caminhos distintos:

Regressão Logística: Utilizada pela sua alta interpretabilidade. Apliquei o StandardScaler para normalizar os dados, já que modelos lineares são sensíveis à escala.

Random Forest: Utilizado para capturar relações não-lineares e interações complexas entre os serviços contratados.

📈 Insights e Resultados
O modelo de Regressão Logística foi o meu escolhido para o relatório final, apresentando um equilíbrio sólido entre acurácia e recall. Algumas das descobertas mais relevantes foram:

Vulnerabilidade no Onboarding: Clientes com menos de 10 meses de contrato representam o maior risco de saída.

Impacto Contratual: A ausência de contratos de fidelidade (anual/bienal) é o principal catalisador do Churn.

Segurança como Retenção: Notei que clientes que utilizam serviços de segurança digital tendem a ter um ciclo de vida muito maior na empresa.

💡 Estratégias Propostas
Com base nos modelos, propus quatro pilares de ação:

Monitoramento Intensivo: Acompanhamento prioritário nos primeiros 6 meses de contrato.

Conversão de Contratos: Incentivos para migração do plano mensal para contratos de fidelidade.

Cross-selling de Segurança: Oferta de pacotes de proteção digital como ferramenta de fidelização.

Ajuste Financeiro: Promoção do débito automático para reduzir o atrito do pagamento manual via boleto.

📂 Como executar o projeto
Clone o repositório.

Certifique-se de ter o arquivo TelecomX_Data.json no diretório raiz.

Execute o notebook TELECOM_ALURA.ipynb em um ambiente Jupyter ou Google Colab.
