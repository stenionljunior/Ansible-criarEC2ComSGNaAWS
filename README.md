# Provisionamento de instância EC2 com SG na AWS utilizando o Ansible

Provisionamento de instância EC2 com Security Group na AWS utilizando o Ansible

## Configuração do ambiente:

Necessário ter instalado o Python, pip e boto na máquina de controle do Ansible.

- instalar o python:

```bash
sudo apt install python
```
- Instalar o pip
```bash
sudo apt install python-pip
```
- Instalar o boto
```bash
pip install boto
```

 
## Configurações para acessar a AWS

Exemplo de configuração utilizando variável de ambiente e utilizando o AWS CLI

- Via variável de ambiente:

```bash
export AWS_ACCESS_KEY_ID='AK123'
export AWS_SECRET_ACCESS_KEY='abc123'
```

- Via AWS CLI:

```bash
apt install awscli
aws configure
```


## Para rodar o playbook na máquina de controle do Ansible.:

```bash
git clone https://github.com/stenionljunior/Ansible-criarEC2ComSGNaAWS.git
cd Ansible-criarEC2ComSGNaAWS/
ansible-playbook -i hosts main.yml
```

## License
[MIT](https://choosealicense.com/licenses/mit/)