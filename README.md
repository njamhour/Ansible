 # Ansible
## Por que Ansible
- **Ferramenta Open Source**
- **Simples (YAML - chave:valor)**
- **Baixa curva de aprendizado**
- **Agentless (Sem agentes - 100% limpa)**
- **Facil de ler(YAML)**

## Informações
- Extremamente recomendado gerar uma chave SSH (RSA) para a agilidade do gerenciamento dos servidores

## Roles (Estrutura)
- **tasks:** lista de tarefas para serem executadas em uma role
- **handlers:** manipuladores/eventos acionados por uma task
- **files:** arquivos utilizados para deploy dentro de um role
- **templates:** modelos para deploy dentro de uma role (permite uso de variaveis)
- **vars:** variaveis adicionais de uma role
- **defaults:** variaveis padrão de uma role. Prioridade máxima
- **meta:** trate dependências de uma role por outr arole - Primeiro diretorio a ser analisado

## Exemplo comandos
 **ansible -i hosts servidores_web -m setup**
 - Realiza o inventario da maquina
