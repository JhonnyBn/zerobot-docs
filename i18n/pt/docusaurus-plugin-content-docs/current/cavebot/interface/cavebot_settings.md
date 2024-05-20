---
sidebar_position: 5
---

# Configurações do CaveBot
## Opções Principais
<div class="text--center">
  <img src="/img/cavebot_settings.png" />
  <p>Configurações do CaveBot</p>
</div>

**Load** -> carrega um CaveBot específico

**Save** -> salva o CaveBot atual

**Settings** -> configurações gerais do CaveBot

## Configurações Avançadas do CaveBot
<div class="text--center">
  <img src="/img/cavebot_settings_window.png" />
  <p>Configurações Avançadas do CaveBot</p>
</div>

### Ignore Lure List
No campo de texto mostrado na imagem acima, por favor insira os nomes dos monstros que o sistema de lure do cavebot deve ignorar. Insira cada nome de monstro em uma linha separada.

### Lure Settings
**Max Lure To Leave**: supondo que seu personagem alcançou o waypoint "End Lure" e está matando os monstros para terminar a lure, esta configuração define quantas criaturas devem restar para considerar a lure concluída e prosseguir para o próximo waypoint. Exemplo: se você definir o valor para 3, então o bot entenderá que deve haver 3 ou menos criaturas restantes para terminar de matar as criaturas e prosseguir.

**Min Lure To Leave**: supondo que seu personagem alcançou o waypoint "End Lure", o bot se baseará nesta configuração para decidir se para seu personagem ou não para matar as criaturas ao redor. Exemplo: se você definir o valor para 3, então o bot só parará para matar as criaturas da lure se houver 3 ou mais criaturas, caso contrário, prossegue normalmente.

**Min Lure To Walk**: supondo que você está atraindo monstros no waypoint "Start Lure", o bot só andará mais rápido e ignorará as criaturas **sem esperar por elas** se alcançar o valor configurado. Exemplo: se você definir o valor para 3, então o bot só andará sem esperar se houver 3 ou mais criaturas, garantindo assim pelo menos 3 criaturas em sua lure

**Avoid Stuck/Trap**: Número mínimo de blocos ao redor do seu personagem em uma área de 1x1 para considerar seguro forçar a caminhada e evitar ficar preso. Para desativar esta funcionalidade, defina como 0.

## Configurações do Auto Recorder
**Distance**: Distância em SQMs entre waypoints gravados automaticamente.

**Type**: O tipo de waypoint dos waypoints gravados automaticamente

## Configurações de Node
**Distância**: A distância entre o jogador e o waypoint 'nó' que o CaveBot considerará como alcançado.