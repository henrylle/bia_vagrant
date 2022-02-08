## Para adicionar acesso remoto ao VS Code do vagrant

[Link para conexão remota via ssh no VS Code](https://medium.com/@lizrice/ssh-to-vagrant-from-vscode-5b2c5996bc0e#:~:text=ssh%2Fconfig%20.,machine%20name%20that%20Vagrant%20assigned)

## Para rodar bia através do vagrant
- Pré-requisitos: Instalar virtualbox e vagrant
- Passo 1: Clona esse projeto
- Passo 2: vagrant up
- Passo 3: vagrant ssh-config (copia esses dados)
- Passo 4: Instala extensão remote explorer no vs code
- Passo 5: Adiciona dados do vagrant para a config
- Passo 6: Abre o terminal dentro vm 
- Passo 7: Clona esse projeto dentro da vm
- Passo 8: chmod +x prepara_linux_vagrant.sh 
- Passo 9: ./prepara_linux_vagrant.sh
- Passo 10: Clonar a bia e dar docker-compose up
