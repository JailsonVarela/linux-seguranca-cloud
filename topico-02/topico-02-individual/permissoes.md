# Permissões aplicadas
## Ambiente utilizado
WSL

## Utilizador e grupos
Inserir output ou resumo dos comandos whoami, id e groups.
whoami -> jailson
id -> uid=1000(jailson) gid=1000(jailson) groups=1000(jailson),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),100(users)
groups -> jailson adm cdrom sudo dip plugdev users

## Ficheiros criados
- publico.txt:
- restrito.txt:
- script.sh:

## Permissões aplicadas
| Ficheiro | Permissão | Justificação |
|---|---|---|
| publico.txt | 644 | Administrador pode ler e escrever, grupos e outros utilizadores podem apenas ler |
| restrito.txt | 640 | Administrador pode ler e escrever, grupos podem ler e outros utilizadore não tem acesso |
| script.sh | u+x | Dá permissão ao administrador para execução. O que resulta no acesso total do administrador, grupos podem ler e escrever e os outros utilizadores podem apenas ler |

## Relação com o princípio do menor privilégio
Explicar por que as permissões aplicadas são mais adequadas do que permissões totais para todos.
As permissões aplicadas são mais indicadas pois restringe o acesso.
