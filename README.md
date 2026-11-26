# Instruções do que se encontra no projeto. *** Importante ***

O 
Objetivo: executar o arquivo nome_do_executavel, uma calculadora básica que exibe informações sobre o diretório em que está e, em seguida, abre a calculadora do sistema operacional.

Passo a passo:

Abra o terminal. Use o atalho Ctrl + Alt + T ou procure por "Terminal" no menu de aplicativos.
Acesse a pasta onde o arquivo está salvo. Use o comando cd seguido do caminho da pasta. Por exemplo:
bash
cd ~/Downloads
Confira se o arquivo está na pasta. Liste o conteúdo do diretório com:
bash
ls
Dê permissão de execução ao arquivo. Por padrão, o Linux não permite executar arquivos baixados. Use:
bash
chmod +x nome_do_executavel
Execute o programa. Digite:
bash
./nome_do_executavel

O que deve acontecer:

O programa exibe no terminal as informações do diretório em que está sendo executado (por exemplo, o caminho atual e os arquivos presentes nele).
Em seguida, a calculadora padrão do Ubuntu é aberta automaticamente, e você pode usá-la normalmente.

Observação: se aparecer a mensagem "Permissão negada", repita o passo 4. Se aparecer "Arquivo ou diretório inexistente", confira se você está na pasta correta (passos 2 e 3).

