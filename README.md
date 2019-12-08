# data-analyst-INEP-ENADE-2009TO2013
<![endif]–>

Algoritmo e Lógica de Programação

Alunos: Daniel e Everton;

Curso: Análise e Desenvolvimento de Sistemas;

Período: 1º Semestre;

Turma: B;

Professor: Eduardo Masanori;

Atividade: EP1: Análise de Dados.

Equipamento utilizado para o trabalho:

<![if !supportLists]>· <![endif]>Nome do Sistema Operacional: Microsoft Windows 7 Professional;

<![if !supportLists]>· <![endif]>Versão: 6.1.7601 Service Pack 1 Compilação 7601;

<![if !supportLists]>· <![endif]>Tipo do sistema: x64-based PC;

<![if !supportLists]>· <![endif]>Processador: Intel® Core™ i5-3210M CPU @ 2.50GHz, 2501 Mhz, 2 Núcleo(s), 4 Processador(es) Lógico(s);

<![if !supportLists]>· <![endif]>Memória Física (RAM) Instalada: 4,00 GB;

<![if !supportLists]>· <![endif]>Memória física total: 3,87 GB.

Dependências para a execução da análise e apresentação das informações:

<![if !supportLists]>· <![endif]>Python:

<![if !supportLists]>o <![endif]>Versão: python-3.7.4-amd64;

<![if !supportLists]>o <![endif]>Download: https://www.python.org/downloads/;

<![if !supportLists]>o <![endif]>Instalação:

<![if !supportLists]>§ <![endif]>Na instalação, habilite a opção Figura1, pacote que permitirá a instalação de pacotes e suas dependências via prompt, e, habilite a opção Figura2, para que os comandos do Python sejam executar em qualquer diretório via prompt.

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image001.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image003.jpg)<![endif]>

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image004.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image006.jpg)<![endif]>

<![if !supportLists]>o <![endif]>Atualização pip:

<![if !supportLists]>§ <![endif]>Abra o prompt de comando:

<![if !supportLists]>· <![endif]>Pressione Tecla Windows + R;

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image007.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image008.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image010.jpg)<![endif]>

<![if !supportLists]>· <![endif]>Digite e pressione enter;

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image012.jpg)<![endif]>

<![if !supportLists]>§ <![endif]>Digite o comando <pip install --upgrade pip> e pressione enter, aguarde a atualização.

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image014.jpg)<![endif]>

<![if !supportLists]>o <![endif]>Instalação das bibliotecas e dependências:

<![if !supportLists]>§ <![endif]>Abra o prompt de comando:

<![if !supportLists]>· <![endif]>Pressione Tecla Windows + R;

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image015.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image016.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image017.jpg)<![endif]>

<![if !supportLists]>· <![endif]>Digite e pressione enter;

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image018.jpg)<![endif]>

<![if !supportLists]>§ <![endif]>Digite o comando e pressione enter, aguarde a instalação dos pacotes.

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image020.jpg)<![endif]>

<![if !supportLists]>o <![endif]>Preparação do ambiente para análise dos dados:

<![if !supportLists]>§ <![endif]>Crie um diretório, selecione o local que desejar. Neste trabalho utilizado o diretório <C:\Analise-Dados-INEP>;

<![if !supportLists]>§ <![endif]>Baixe os arquivos ‘.CSV’ para análise. Arquivos estão disponíveis em:

<![if !supportLists]>· <![endif]>https://drive.google.com/file/d/1IOG8BEshJLGOQG2Eg84v8UMPeSATbiJ4/view?usp=sharing

<![if !supportLists]>· <![endif]>Neste trabalho serão analisados os anos de 2009 há 2013.

<![if !supportLists]>§ <![endif]>Extraia os arquivos dentro do diretório <C:\Analise-Dados-INEP\Dados>;

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image021.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image022.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image024.jpg)<![endif]>

<![if !supportLists]>o <![endif]>Executar o Jupyter Notebook:

<![if !supportLists]>§ <![endif]>Abra o prompt de comando:

<![if !supportLists]>· <![endif]>Pressione Tecla Windows + R;

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image025.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image026.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image027.jpg)<![endif]>

<![if !supportLists]>· <![endif]>Digite e pressione enter;

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image028.jpg)<![endif]>

<![if !supportLists]>§ <![endif]>Acesse o diretório <C:\Analise-Dados-INEP>, digite o comando <cd C:\Analise-Dados-INEP> e pressione enter;

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image030.jpg)<![endif]>

<![if !supportLists]>§ <![endif]>Digite o comando , será executado em servidor de web com os recursos para a realização das análises, aguarde a execução do servidor e não feche o cmd, abrirá a janela do navegador padrão com o serviço Jupyter Notebook.

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image032.jpg)<![endif]>

Obs. Caso não abra o navegador padrão com o acesso ao Jupyter Notebook, copie e cole no navegador padrão e URL e de acesso, conforme figura abaixo:

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image033.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image035.jpg)<![endif]>

No computador gerou a URL “http://localhost:8888/?token=b0440a6dff3b806f3592b58797390fabdf6d1dddf645c957”, copie a URL gerada e cole no navegador padrão e pressione enter que abrirá os recursos do Jupyter Notebook, conforme imagem abaixo:

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image037.jpg)<![endif]>

<![if !supportLists]>o <![endif]>Iniciar a análise de dados:

<![if !supportLists]>§ <![endif]>Clique em <New\Python 3>, conforme figura abaixo:

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image038.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image039.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image041.jpg)<![endif]>

<![if !supportLists]>§ <![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image042.png)<![endif]>Na nova janela que abrira renomeie o arquivo para o nome desejado, neste trabalho utilizado o nome “data-analyst-INEP-ENADE-2009TO2013”, conforme figura abaixo:

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image043.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image045.jpg)<![endif]>

<![if !supportLists]>§ <![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image046.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image047.png)<![endif]>Inserir as células e executá-las, para adicionar pressione o botão (+) e para executar pressione o botão (>| Run), da paleta de comandos, conforme figura abaixo:

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image049.jpg)<![endif]>

<![if !supportLists]>· <![endif]>Import das bibliotecas:

#import das bibliotecas necessárias para o desenvolvimento do EP

import pandas as pd

import matplotlib.pyplot as plt

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image050.png)<![endif]><![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image052.jpg)<![endif]>

Atenção: Caso apareça um asterisco entre colchetes, significa que o comando está em execução, caso seja representado numericamente, significa que o comando foi executado, caso apareça em branco, significa que os comandos contidos na célula não foram executados.

<![if !supportLists]>· <![endif]>Configurações iniciais:

#configurações iniciais

low_memory=False

pd.options.display.max_columns = 80

pd.options.display.max_rows = 90

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image054.jpg)<![endif]>

<![if !supportLists]>· <![endif]>Declaração das variáveis:

#declaração variáveis

d = ‘./Dados/’

pN = ‘DM_ALUNO_’

anos = [‘2009’, ‘2010’, ‘2011’, ‘2012’, ‘2013’]

e = ‘.CSV’

dm = ‘DM.CSV’

dados = []

dadosFe = []

dadosEs = []

dadosMu = []

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image056.jpg)<![endif]>

<![if !supportLists]>· <![endif]>Criação do Data Frame e Leitura dos arquivos, quantificando os dados e armazenando-os em suas respectivas listas:

for ano in anos:

df = pd.read_csv(d+pN+ano+e, usecols=[‘CO_COR_RACA_ALUNO’, ‘CO_CATEGORIA_ADMINISTRATIVA’], delimiter = ‘|’, encoding = ‘iso-8859-1’)

#contabilização e consolidação das informações - Geral

dados.append(df.query(’(CO_COR_RACA_ALUNO == 2 or CO_COR_RACA_ALUNO == 3) and (CO_CATEGORIA_ADMINISTRATIVA == 1 | CO_CATEGORIA_ADMINISTRATIVA == 2 | CO_CATEGORIA_ADMINISTRATIVA == 3)’)[‘CO_COR_RACA_ALUNO’].count())

#contabilização e consolidação das informações - Federal

dadosFe.append(df.query(’(CO_COR_RACA_ALUNO == 2 or CO_COR_RACA_ALUNO == 3) and (CO_CATEGORIA_ADMINISTRATIVA == 1)’)[‘CO_COR_RACA_ALUNO’].count())

#contabilização e consolidação das informações - Estadual

dadosEs.append(df.query(’(CO_COR_RACA_ALUNO == 2 or CO_COR_RACA_ALUNO == 3) and (CO_CATEGORIA_ADMINISTRATIVA == 2)’)[‘CO_COR_RACA_ALUNO’].count())

#contabilização e consolidação das informações - Municipal

dadosMu.append(df.query(’(CO_COR_RACA_ALUNO == 2 or CO_COR_RACA_ALUNO == 3) and (CO_CATEGORIA_ADMINISTRATIVA == 3)’)[‘CO_COR_RACA_ALUNO’].count())

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image058.jpg)<![endif]>

<![if !supportLists]>· <![endif]>Plotar dados sintéticos obtidos no gráfico:

#plotar dados gráfico

fig, ax = plt.subplots()

plt.rcParams[‘figure.figsize’] = (10,8)

ax.plot(anos, dados, label=‘Total’)

ax.plot(anos, dadosFe, label=‘Federal’)

ax.plot(anos, dadosEs, label=‘Estadual’)

ax.plot(anos, dadosMu, label=‘Municipal’)

ax.grid()

plt.legend()

plt.title(‘Evolução: Negros (Pretos e Pardos) ingressantes em Universidades Públicas’)

plt.xlabel(‘Anos’)

plt.ylabel(‘Quantidade’)

plt.show()

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image060.jpg)<![endif]>

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image062.jpg)<![endif]>

<![if !supportLists]>· <![endif]>Consolidação dos resultados:

#organização dos dados em tabelas, para melhor visualização dos dados

consolidacao = {

‘2009’: [dadosFe[0], dadosEs[0], dadosMu[0], dados[0]],

‘2010’: [dadosFe[1], dadosEs[1], dadosMu[1], dados[1]],

‘2011’: [dadosFe[2], dadosEs[2], dadosMu[2], dados[2]],

‘2012’: [dadosFe[3], dadosEs[3], dadosMu[3], dados[3]],

‘2013’: [dadosFe[4], dadosEs[4], dadosMu[4], dados[4]],

}

df_DC = pd.DataFrame(consolidacao, columns=anos, index=[‘Federal’,‘Estadual’,‘Municipal’,‘Total’])

df_DC

<![if !vml]>![](file:///C:/Users/tomsa/AppData/Local/Packages/oice_16_974fa576_32c1d314_2d4f/AC/Temp/msohtmlclip1/01/clip_image064.jpg)<![endif]>
