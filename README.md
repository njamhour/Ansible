 '# Ansible' 
Por que Ansible
- Ferramenta Open Source
- Simples (YAML - chave:valor)
- Baixa curva de aprendizado
- Agentless (Sem agentes - 100% limpa)
- Facil de ler(YAML)

'#Roles'
tasks - lista de tarefas para serem executadas em uma role
handlers - manipuladores/eventos acionados por uma task
files - arquivos utilizados para deploy dentro de um role
templates - modelos para deploy dentro de uma role (permite uso de variaveis)
vars - variaveis adicionais de uma role
defaults - variaveis padrão de uma role. Prioridade máxima
meta - trate dependências de uma role por outr arole - Primeiro diretorio a ser analisado
