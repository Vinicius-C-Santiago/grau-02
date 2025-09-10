#1. instalar openSSH
sudo apt-get update
sudo apt-get install openssh-server
#verificar status do serviço
sudo systemctl status ssh

#2. acessar ssh
ssh nome_usuario@ip_do_usuario
#confirmar a autenticação do host
yes
#colocar senha
senha

#3. configuração de segurança
sudo cp /etc/ssh/sshd_config /etc/ssh/sshd_config
sudo nano /etc/ssh/sshd_config
#alterar porta
#port 22 -> port 2244
#desabilitar login de root
PermitRootLogin no
#salvar e fechar arquivo
Ctrl+O, Enter, Ctrl+x
