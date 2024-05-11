# Projeto_ImersaoIA
Assistente de Estudos para alunos do Ensino Médio.

Uma dificuldade no Ensino é assistir aos alunos que, por motivos diversos, faltaram e, também, aqueles que são muitos tímidos e não perguntam durante as aulas, mas estão com muitas dúvidas. Criei um código para auxiliá-los em seus estudos, usando o Gemini. Como não tenho experiência em Python, me restringi às funções que foram apresentadas na Semana de ImersãoIA. Futuramente, pode-se ampliar a aplicação, incluindo mais recursos e finalidades, além de adaptá-lo para outras etapas e cursos de Ensino. Espero que gostem!

Comentários:
Este código Python demonstra como usar o Google Generative AI para criar um assistente de estudos interativo. Ele usa a biblioteca google-generativeai para interagir com a API do Google e gerar texto de alta qualidade em resposta às dúvidas dos usuários sobre diferentes disciplinas.

Passo a Passo:
Instalação e Importação:

Instala a biblioteca google-generativeai usando pip.
Importa as bibliotecas necessárias, incluindo google.generativeai e google.colab.userdata.

Configuração da API:
Define a chave da API obtida do Google Cloud Platform usando userdata.get("secret_key").
Configura a API usando genai.configure(api_key=api_key).

Configurações de Geração e Segurança:
Define parâmetros para controlar a criatividade, probabilidade de palavras e tamanho máximo da saída do modelo de linguagem.
Define configurações de segurança para bloquear conteúdo ofensivo, discurso de ódio, conteúdo sexualmente explícito e conteúdo perigoso.

Inicialização do Modelo:
Cria uma instância do modelo generativo (gemini-1.5-pro-latest) usando as configurações especificadas.

Interação com o Usuário:
Apresenta uma mensagem de boas-vindas e uma lista de disciplinas disponíveis.
Solicita ao usuário que escolha uma disciplina, insira o conteúdo de estudo e faça uma pergunta.

Geração da Resposta:
Constrói um prompt para o modelo com base na disciplina, conteúdo e dúvida do usuário.
Usa model.generate_content(prompt) para gerar uma resposta.

Esclarecimento da Dúvida:
Pergunta ao usuário se a resposta esclareceu sua dúvida.
Oferece opções para gerar respostas mais simples ou mais aprofundadas, dependendo do feedback do usuário.

Encerramento:
Exibe uma mensagem de encerramento quando a dúvida do usuário é esclarecida.

Observações:
Certifique-se de ter uma chave de API válida do Google Cloud Platform.
Ajuste as configurações de geração e segurança de acordo com suas necessidades.
Este código é um exemplo básico e pode ser expandido para incluir mais recursos e funcionalidades, como suporte a diferentes idiomas, personalização de respostas e integração com outras ferramentas.
