Analise-Dados-INEP
Análise de dados INEP ENAD, negros (Pretos e Pardos) ingressantes a faculdades públicas no BRASIL.

Equipamento utilizado:
Nome do Sistema Operacional: Microsoft Windows 7 Professional;
Versão: 6.1.7601 Service Pack 1 Compilação 7601;
Tipo do sistema: x64-based PC;
Processador: Intel(R) Core(TM) i5-3210M CPU @ 2.50GHz, 2501 Mhz, 2 Núcleo(s), 4 Processador(es) Lógico(s);
Memória Física (RAM) Instalada: 4,00 GB;
Memória física total: 3,87 GB.
Dependências para a execução da análise e apresentação das informações:
Python:

Versão: python-3.7.4-amd64;
Download: Link download Pyton;
Instalação:
Na instalação, habilite a opção (pip) Figura - 1, pacote que permitirá a instalação de pacotes e suas dependências via prompt, e, habilite a opção Add python to environment variables Figura - 2, para que os comandos do Python sejam executar em qualquer diretório via prompt.
Imagem de habilitar o PIP

Imagem de habilitar o PATH

Atualização pip:
Abra o prompt de comando:
Pressione Tecla Windows + R, Figura - 3;
Imagem teclado

Digite (cmd) e pressione enter, Figura - 4;
Imagem janela executar

Digite o comando (pip install --upgrade pip) e pressione enter, aguarde a atualização, Figura - 5.
Imagem cmd upgrade PIP  

Instalação das bibliotecas e dependências:
Abra o prompt de comando:
Pressione Tecla Windows + R, Figura - 6;
Imagem teclado

Digite (cmd) e pressione enter, Figura - 7;
Imagem janela executar

Digite o comando:
pip install requests beautifulsoup4 spotipy pdfminer3k selenium twitter wbdata pandas matplotlib lxml tweepy uber-rides xlrd PyPDF2 pytrends seaborn numpy ipython jupyter twitter-scraper markovify folium
Pressione enter, aguarde a instalação dos pacotes, Figura - 8.
Imagem cmd PIP instalação dependências

Preparação do ambiente para análise dos dados:
Crie um diretório, selecione o local que desejar. Neste trabalho utilizado o diretório (C:\Analise-Dados-INEP>);
Baixe os arquivos ‘.CSV’ para análise. Arquivos estão disponíveis em:
Link download Dados
Neste trabalho serão analisados os anos de 2009 há 2013.
Extraia os arquivos dentro do diretório (**C:\Analise-Dados-INEP\Dados**), Figura - 9;
Imagem cmd dir Dados

Executar Jupyter Notebook:
Abra o prompt de comando:
Pressione Tecla Windows + R, Figura - 10;
Imagem teclado

Digite (cmd) e pressione enter, Figura - 11;
Imagem janela executar

Acesse o diretório (**C:\Analise-Dados-INEP**), digite o comando (cd C:\Analise-Dados-INEP>) e pressione enter, Figura - 12;
Imagem cmd cd Diretório execução Jupyter

Digite o comando (jupyter notebook), será executado em servidor de web com os recursos para a realização das análises, aguarde a execução do servidor e não feche o cmd, abrirá a janela do navegador padrão com o serviço Jupyter Notebook, Figura - 13.
Imagem cmd run Jupyter Notebook

Obs. Caso não abra o navegador padrão com o acesso ao Jupyter Notebook,
copie e cole no navegador padrão e URL e de acesso, **Figura - 14**:
Imagem copiar URL

No computador gerou a URL “http://localhost:8888/?token=b0440a6dff3b806f3592b58797390fabdf6d1dddf645c957”,
copie a URL gerada e cole no navegador padrão e pressione enter que abrirá os recursos do Jupyter Notebook, **Figura - 15**:
Imagem Browser - Pagina Inicial Jupyter

Iniciar a análise de dados:
Clique em (New\Python 3), Figura - 16:
Imagem Browser - Novo arquivo Python 3

Na nova janela que abrira renomeie o arquivo para o nome desejado, neste trabalho utilizado o nome “data-analyst-INEP-ENADE-2009TO2013”, Figura - 17:
Imagem Browser - Renomear arquivo

Inserir as células e executá-las, para adicionar pressione o botão (+) e para executar pressione o botão (>| Run), da paleta de comandos, Figura - 18:
Imagem Browser - Comandos

Import das bibliotecas:
#import das bibliotecas necessárias para o desenvolvimento do EP
import pandas as pd
import matplotlib.pyplot as plt
Imagem Browser - Input Import

Atenção: Caso apareça um asterisco entre colchetes, significa que o comando está em execução,
caso seja representado numericamente, significa que o comando foi executado, caso apareça em branco,
significa que os comandos contidos na célula não foram executados.
Configurações iniciais:
#configurações iniciais
low_memory=False
pd.options.display.max_columns = 80
pd.options.display.max_rows = 90
Imagem Browser - Input Configurações Iniciais

Declaração das variáveis:
#declaração variáveis
d = './Dados/'
pN = 'DM_ALUNO_' 
anos = ['2009', '2010', '2011', '2012', '2013'] 
e = '.CSV'
dados = []
dadosFe = []
dadosEs = []
dadosMu = []
Imagem Browser - Input Declaração Variáveis

 

Criação do Data Frame e Leitura dos arquivos, quantificando os dados e armazenando-os em suas respectivas listas:
#criação do Data Frame e Leitura dos arquivos, contando os dados e armazená-los nas respectivas listas
for ano in anos:
    df = pd.read_csv(d+pN+ano+e, usecols=['CO_COR_RACA_ALUNO', 'CO_CATEGORIA_ADMINISTRATIVA'], delimiter = '|', encoding = 'iso-8859-1')
    #contabilização e consolidação das informações - Geral
    dados.append(df.query('(CO_COR_RACA_ALUNO == 2 or CO_COR_RACA_ALUNO == 3) and (CO_CATEGORIA_ADMINISTRATIVA == 1 | CO_CATEGORIA_ADMINISTRATIVA == 2 | CO_CATEGORIA_ADMINISTRATIVA == 3)')['CO_COR_RACA_ALUNO'].count()) 
    #contabilização e consolidação das inforamções - Federal
    dadosFe.append(df.query('(CO_COR_RACA_ALUNO == 2 or CO_COR_RACA_ALUNO == 3) and (CO_CATEGORIA_ADMINISTRATIVA == 1)')['CO_COR_RACA_ALUNO'].count()) 
    #contabilização e consolidação das informações - Estadual
    dadosEs.append(df.query('(CO_COR_RACA_ALUNO == 2 or CO_COR_RACA_ALUNO == 3) and (CO_CATEGORIA_ADMINISTRATIVA == 2)')['CO_COR_RACA_ALUNO'].count()) 
    #contabilização e consolidação das informações - Municipal
    dadosMu.append(df.query('(CO_COR_RACA_ALUNO == 2 or CO_COR_RACA_ALUNO == 3) and (CO_CATEGORIA_ADMINISTRATIVA == 3)')['CO_COR_RACA_ALUNO'].count())
Imagem Browser - Input Data Frame  

Plotar dados sintéticos obtidos no gráfico:
#plotar dados gráfico
fig, ax = plt.subplots()
plt.rcParams['figure.figsize'] = (10,8)
ax.plot(anos, dados, label='Total')
ax.plot(anos, dadosFe, label='Federal')
ax.plot(anos, dadosEs, label='Estadual')
ax.plot(anos, dadosMu, label='Municipal')
ax.grid()
plt.legend()
plt.title('Evolução: Negros (Pretos e Pardos) ingressantes em Universidades Públicas')
plt.xlabel('Anos')
plt.ylabel('Quantidade')
plt.show()
Imagem Browser - Input Plotar Grafico

Imagem Browser - Plotar Grafico

 

Consolidação dos resultados:
#organização dos dados em tabelas, para melhor visualização dos dados
consolidacao = {}
for x in range(5):    
    consolidacao.update({anos[x]: [dadosFe[x], dadosEs[x], dadosMu[x], dados[x]],})
df_DC = pd.DataFrame(consolidacao, columns=anos, index=['Federal','Estadual','Municipal','Total'])
df_DC
Imagem Browser - Input e Tabela Resultados
