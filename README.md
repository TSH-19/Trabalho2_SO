

# Trabalho2_SO ( Simulação de Jogo de Futebol com Semáforos e Memória Partilhada )

Este projeto simula um jogo de futebol utilizando processos independentes para representar jogadores, guarda-redes e um árbitro. A sincronização é feita através de semáforos e memória partilhada, garantindo que as regras do jogo são respeitadas e que os processos comunicam de forma coordenada.

---

## Estrutura do Projeto

O projeto é composto pelos seguintes ficheiros:

- **`probConst.h`**: Define as constantes globais do programa.
- **`probDataStruct.h`**: Contém as estruturas de dados partilhadas utilizadas na simulação.
- **`logging.c`**: Gere o registo do estado do sistema em ficheiros de log.
- **`semSharedWatcher.c`**: Implementa as ações do ciclo de vida dos guarda-redes.
- **`semSharedMemSmoker.c`**: Implementa as ações do ciclo de vida dos jogadores.
- **`semSharedMemAgent.c`**: Implementa as ações do ciclo de vida do árbitro.
- **`sharedMemory.h`** e **`semaphore.h`**: Contêm as funções auxiliares para manipulação de semáforos e memória partilhada.

---

## Como Compilar e Executar

Para compilar o projeto, entra na pasta src, utilize o seguinte comando na linha de comandos:

```bash
make all
```
Para limpar todos os arquivos compilados, use:
```bash
make cleanall
```

Para executar o programa compilado entre na pasta run, utilize o seguinte comando na linha de comandos:
```bash
./probSemSharedMemSoccerGame 
```
