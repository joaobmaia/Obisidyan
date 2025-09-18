ls -la(llistar): Lista os arquivos e pastas do diretório atual. 
cd (navegar): cd ..(volta pasta) cd ~(pasta home)
pwd: Mostrar endereço que estou. 
git status: Mostrar quais arquivos foram modificados/adicionados
 🟥 Modificado mas não adicionei ao diretório (Geralmente Untruked) 
 🟩Adicionado ao diretório, pronto para commit. (Geralmente Trunked)
 git add -> adiciona todos os arquivos (até os untrukeds- não conhecidos)
 git -a -> adiciona todos os arquivos trunkados(ja conhecidos)
 git add "Arquivo"
 git commit -m: "Salvar o jogo" e comentar oq vc fez de novo. 
 git commit: Comentar em detalhes o que você mudou nesse novo save. 
 git config --global safe.directory ' /caminho': git pode confiar naquela pasta. 
 termux-setup-storage: Pede permissão para acessar armazenamento do Android -> Resulta na criação da pasta storage com links para sua pasta. 
 Chmod +x: Torna um arquivo executável (x=permite a execução)

#ecoar - imprimir.
echo "Texto"          # Mostra texto na tela
echo "texto" > arquivo # Cria arquivo com texto
echo "texto" >> arquivo # Adiciona texto no final do arquivo

#navegação
pwd                 # Mostra onde estou
ls                  # Lista arquivos
ls -la              # Lista detalhada
cd "pasta"          # Entra na pasta
cd ..               # Volta uma pasta
cd ~                # Vai para home

#gitbasico 
git init            # Iniciar repositório
git status          # Ver situação
git add .           # Adicionar tudo
git add "arquivo"   # Adicionar específico
git commit -m "msg" # Commitar com mensagem
git commit          # Commitar (abre editor)
git log --oneline   # Ver histórico

#gitavancado
git rm "arquivo"    # Remover arquivo
git rm --cached     # Remover só do Git
git mv "old" "new"  # Renomear/mover
git config --global --add safe.directory "/caminho" # Resolver permissão

*Manipulação de Arquivos*
touch arquivo       # Criar arquivo vazio
cat arquivo         # Ver conteúdo
nano arquivo        # Editar arquivo
echo "texto" >> arquivo # Adicionar texto

**Links e a Atalhos**
ln -s "/caminho/longo" ~/atalho # Criar atalho
termux-setup-storage   # Pedir acesso ao armazenamento

