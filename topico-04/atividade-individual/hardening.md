\##Identificar se o serviço publicado usa Nginx, Apache ou WordPress.
O serviço indicado usa Nginx como servidor para publicar o serviço web.


##Listar riscos específicos desse serviço.
Os riscos especificos são permissões exageradas.


##Propor medidas iniciais de hardening.
Como medidas iniciais propõe se a revisão da checklist:

1. Atualizar os pacotes
2. Rever serviços ativos
3. Reduzir permissões aplicando o  principio do menor privilégio
4. Proteger dados sensíveis por exemplo /tmp
5. Evitar uso direto do root
6. Documentar alterações


##Indicar que medidas podem ser aplicadas agora.
Agora podem ser aplicadas todas as medidas acima mencionadas:

1. Atualizar os pacotes com sudo apt update e sudo apt upgrade
2. Rever serviços ativos sudo systemctl status
3. Configurar permissões do tmp noexec, nosuid e nodev.


##Indicar que medidas ficam para tópicos seguintes.
Medidas de auditoria com ferramentas:

1. Lynis - analisa o sistema em busca de falhas e sugere melhorias
2. Fail2Ban -permite bloquear tentativas de acesso via força bruta

