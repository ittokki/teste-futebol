<!--
README - INSTRUÇÕES DE USO DO DASHBOARD

Bem-vindo ao Dashboard de Jogadores! Este é um arquivo HTML único e autônomo.
Para usá-lo, basta abri-lo em qualquer navegador moderno (Chrome, Firefox, Edge).

CONFIGURAÇÃO INICIAL (API DO GOOGLE SHEETS):

Este arquivo já está pré-configurado com a API Key e o ID da Planilha que você forneceu.

Para usar uma planilha diferente, edite as seguintes variáveis no código JavaScript abaixo (procure por "CONFIGURAÇÕES PRINCIPAIS"):

apiKey: Sua chave de API do Google Cloud Platform com acesso à API do Google Sheets.

spreadsheetId: O ID da sua planilha. Você pode encontrá-lo na URL da planilha.

rangePagina1: O intervalo para os dados agregados dos jogadores (ex: 'Página1!A2:H100').

rangePagina2: O intervalo para os dados brutos das partidas (ex: 'Página2!A2:K300').

USO OFFLINE / FALLBACK COM ARQUIVO CSV/EXCEL:

Se a conexão com a API do Google Sheets falhar ou se você estiver offline, uma área para upload de arquivos aparecerá.

Você pode carregar os dados das duas abas da sua planilha como arquivos CSV ou Excel.

Após o upload, você precisará mapear as colunas do seu arquivo para as colunas esperadas pelo dashboard.

Para testar offline, você pode usar os dados de exemplo abaixo.

FOTOS DOS JOGADORES:

As fotos são carregadas a partir do objeto playerPhotos. As URLs que você forneceu já estão no código.

Para adicionar ou alterar uma foto, edite este objeto, associando o NOME NORMALIZADO do jogador à URL da imagem.
&quot;NOME NORMALIZADO&quot;: &quot;URL_DA_FOTO.jpg&quot;

DADOS DE EXEMPLO PARA TESTE OFFLINE:

Copie e cole os dados abaixo em dois arquivos CSV separados (ex: pagina1.csv e pagina2.csv) para usar no modo de upload.

--- Exemplo para Página1 (Jogadores) ---
id,nome,jogos,vitorias,gols,assistencias,golsTomados,golsContra
1,HENRIQUE AMARAL,25,15,30,12,0,1
2,VITOR,22,10,5,8,35,0
3,MARCO DAITX,28,18,25,20,0,2
4,EDUARDO DUDU,20,12,15,10,0,0
5,WILIAN SILVA,26,16,10,15,0,1

--- Exemplo para Página2 (Partidas) ---
nomeRaw,gols,assistencias,golsTomados,golsContra,notaADM,dataJogo,vitoriaRaw,time,resultado,jogoAconteceuRaw
HENRIQUE AMARAL,2,1,0,0,8,23/07/2024,vitoria,A,5x2,sim
VITOR (GOL),0,0,2,0,7,23/07/2024,vitoria,A,5x2,sim
MARCO DAITX,1,2,0,0,9,23/07/2024,vitoria,A,5x2,sim
EDUARDO DUDU,1,0,0,1,6,23/07/2024,derrota,B,2x5,sim
WILIAN SILVA,1,2,0,0,8.5,23/07/2024,derrota,B,2x5,sim

FUNCIONALIDADES:

Navegue pelas abas "Rankings", "Gráficos", "Hall da Fama" e "Partidas".

Filtre os rankings por mês na aba "Rankings".

Clique em um jogador para ver detalhes, incluindo estatísticas, últimas partidas, conquistas e um gráfico de evolução.

Clique em uma partida para ver os detalhes completos do jogo, incluindo estatísticas individuais.

Use o botão no canto superior direito para alternar entre os temas claro e escuro.

O botão "Exportar para CSV" permite baixar os dados da tabela visível.
-->
