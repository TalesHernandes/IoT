Monitoramento Climático de São Paulo e Rio de Janeiro

Este repositório contém os códigos de simulação de condições climáticas para as cidades de São Paulo e Rio de Janeiro utilizando o Wokwi, além do arquivo JSON para configuração do Node-RED, que permite o processamento dos dados e a visualização dos resultados. O projeto tem como objetivo comparar as temperaturas reais coletadas pela API OpenWeather com os valores ideais de temperatura para essas cidades, conforme os padrões definidos pelo Governo do Estado de São Paulo, e destacar as discrepâncias que indicam a presença de ilhas de calor e outros efeitos ambientais prejudiciais.
Estrutura do Repositório

    wokwi_simulation_sp.ino: Código do Wokwi que simula as condições climáticas ideais para São Paulo.
    wokwi_simulation_rj.ino: Código do Wokwi que simula as condições climáticas ideais para o Rio de Janeiro.
    node-red-flow.json: Arquivo de configuração do Node-RED, que processa os dados de temperatura e outros sensores, e os envia ao banco de dados para visualização no Grafana.

Tecnologias Utilizadas

    Wokwi: Plataforma de simulação de IoT para testar e validar projetos baseados em microcontroladores como o ESP32.
    Node-RED: Plataforma de desenvolvimento baseada em fluxo para integrar e processar dados, utilizando o protocolo MQTT para comunicação com o ESP32.
    OpenWeather API: API que fornece dados meteorológicos em tempo real, utilizados para comparação com as condições simuladas.
    MQTT: Protocolo de mensagens leve para comunicação em tempo real entre os dispositivos e o servidor.
    InfluxDB: Banco de dados para armazenamento de séries temporais, utilizado para registrar as medições de temperatura.
    Grafana: Ferramenta de visualização de dados para criar dashboards interativos e exibir os resultados obtidos.

Objetivo do Projeto

Este projeto visa monitorar as condições climáticas de São Paulo e Rio de Janeiro, comparando os dados de temperatura em tempo real com os valores ideais definidos pelo Governo do Estado de São Paulo para identificar discrepâncias que podem ser atribuídas a problemas como ilhas de calor e poluição. Através da integração de tecnologias como IoT, MQTT, Node-RED, InfluxDB e Grafana, buscamos promover a conscientização pública sobre as mudanças climáticas e incentivar ações em direção à sustentabilidade.
Como Usar
Pré-requisitos

    Wokwi: Acesse a plataforma Wokwi e carregue os códigos de simulação.
    Node-RED: Importe o arquivo node-red-flow.json para a sua instância do Node-RED.
    OpenWeather API: Inscreva-se na API do OpenWeather para obter uma chave de API e configure-a no seu código ou fluxo do Node-RED.
    MQTT Broker: Utilize um broker MQTT como o HiveMQ para gerenciar a comunicação entre os dispositivos e o servidor.

Passos

    Simulação no Wokwi: Carregue os códigos de simulação para São Paulo e Rio de Janeiro na plataforma Wokwi, que vai simular as condições ideais de temperatura para ambas as cidades.
    Configuração do Node-RED: Importe o arquivo JSON para configurar os fluxos que processam os dados obtidos do ESP32, enviam os dados para o banco de dados InfluxDB e geram alertas em caso de discrepâncias nas temperaturas.
    Visualização: Utilize o Grafana para exibir os dados em tempo real, criando dashboards interativos que mostram as condições climáticas de ambas as cidades e as comparações com os valores ideais de temperatura.

Resultados Esperados

Ao rodar a simulação e visualizar os dados, será possível observar as discrepâncias entre as temperaturas ideais e as reais, o que ajudará a identificar potenciais problemas relacionados ao aquecimento urbano e à qualidade do ar, como as ilhas de calor.
Contribuições

Contribuições para o aprimoramento deste projeto são bem-vindas! Se você tem sugestões de melhorias, correções de bugs ou novos recursos, sinta-se à vontade para abrir um Pull Request ou um Issue.
Licença

Este projeto está licenciado sob a MIT License.
