 # Ansible
## Por que Ansible
- **Ferramenta Open Source**
- **Simples (YAML - chave:valor)**
- **Baixa curva de aprendizado**
- **Agentless (Sem agentes - 100% limpa)**
- **Facil de ler(YAML)**

## Informações
- Extremamente recomendado gerar uma chave SSH (RSA) para a agilidade do gerenciamento dos servidores
### Ordem de execução
- 1. defaults/main.yml
- 2. host_var/www
- 3. inventory (variaveis de hosts)
- 4. group_vars/servidores
- 5. inventory (variaveis de grupos)
## Roles (Estrutura)
- **tasks:** lista de tarefas para serem executadas em uma role
- **handlers:** manipuladores/eventos acionados por uma task
- **files:** arquivos utilizados para deploy dentro de um role
- **templates:** modelos para deploy dentro de uma role (permite uso de variaveis)
- **vars:** variaveis adicionais de uma role
- **defaults:** variaveis padrão de uma role. Prioridade máxima
- **meta:** trata dependências de uma role por outra role - **Primeiro diretorio a ser analisado**

## Exemplo comandos
 - ansible -i hosts servidores_web -m setup
 **Realiza o inventario da maquina**
 - ansible -i hosts all -m ping
**Verifica se os hosts estão UP**
