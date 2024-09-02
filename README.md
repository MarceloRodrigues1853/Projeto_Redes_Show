# 🌟 Projeto de Redes Estrela para o Show 🎤

Este projeto foi desenvolvido para configurar uma **topologia de rede estrela** que permite a comunicação eficiente entre os membros da equipe de produção de um show. O projeto foi criado utilizando o **Cisco Packet Tracer**.

## 📋 Roteiro do Projeto

### 1. Definir o Cenário
Imagine que a equipe de produção tem quatro membros, cada um com seu próprio computador. Eles precisam se comunicar entre si durante o show, então você vai configurar uma rede para isso.

### 2. Montar a Topologia no Cisco Packet Tracer
- Abra o **Cisco Packet Tracer**.
- Crie uma nova topologia:
  - Arraste um **switch** para o centro da área de trabalho.
  - Arraste **quatro PCs** para a área de trabalho e posicione-os ao redor do switch, formando uma estrela.

### 3. Conectar os Dispositivos
- Conecte cada **PC ao switch** usando cabos ethernet:
  - Selecione o cabo de **cobre direto (Copper Straight-Through)** no Cisco Packet Tracer.
  - Conecte uma extremidade do cabo à interface Ethernet de cada PC e a outra extremidade a uma porta disponível no switch.

### 4. Configurar os Endereços IP
- Atribua endereços IP a cada PC:
  - Clique em cada PC, vá até a aba **Desktop**, selecione **IP Configuration**.
  - Atribua um endereço IP para cada PC dentro da mesma sub-rede. Por exemplo:
    - **PC1:** `192.168.1.1`
    - **PC2:** `192.168.1.2`
    - **PC3:** `192.168.1.3`
    - **PC4:** `192.168.1.4`
  - A máscara de sub-rede deve ser a mesma para todos (por exemplo, `255.255.255.0`).

- **Configuração do Switch:**
  - O switch não precisa de um IP, pois está funcionando como um dispositivo de camada 2, mas se precisar configurá-lo, você pode atribuir um IP à VLAN padrão do switch.

### 5. Testar a Comunicação
- Abra o **Prompt de Comando** em um dos PCs:
  - Vá até a aba **Desktop** de um PC e selecione **Command Prompt**.
  - Use o comando `ping` para testar a comunicação com os outros PCs. Por exemplo:
    - `ping 192.168.1.2`
    - `ping 192.168.1.3`
    - `ping 192.168.1.4`
  - Se tudo estiver configurado corretamente, você deve receber respostas de todos os outros PCs.

## 🌐 Topologia da Rede

A rede configurada é composta por um **switch central** que conecta quatro PCs, representando os membros da equipe de produção. A topologia foi construída para garantir que todos os membros possam se comunicar facilmente durante o evento.

### 📂 Arquivos do Projeto

- **`cisco_TP01.PNG`**: Imagem da topologia da rede.
- **`cisco_TP01-test.PNG`**: Imagem dos testes de ping realizados entre os PCs.
- **`Projeto_PROZ-cisco.pkt`**: Arquivo do Cisco Packet Tracer com a configuração da rede.

## 🔍 Testes de Conectividade

Os testes de ping foram realizados para garantir que todos os PCs possam se comunicar corretamente. A imagem `cisco_TP01-test.PNG` mostra o sucesso dos testes.

## 🚀 Como Executar

1. Abra o **Cisco Packet Tracer**.
2. Importe o arquivo **`Projeto_PROZ-cisco.pkt`**.
3. Verifique a topologia e teste a conectividade entre os PCs usando o comando `ping`.
