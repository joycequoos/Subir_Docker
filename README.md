# Subir Docker

[← Voltar à Trilha de Airflow](https://github.com/joycequoos/Apache_Airflow./blob/main/README.md)

<!--
  Comentário: mesma estrutura início/meio/fim dos READMEs anteriores.
  O conteúdo original era bem curto (3 passos soltos) — mantive a
  essência, só dei um título a cada etapa e adicionei um contexto de
  "quando usar isso", que não estava explícito no README original.
-->

Caso a máquina seja desligada, a conexão do Docker com o Airflow é perdida. Este repositório documenta o procedimento rápido para restabelecer essa conexão.

---

## Quando usar este procedimento

Use este passo a passo sempre que:

- A máquina for desligada ou reiniciada.
- O Docker Desktop não estiver mais rodando.
- Você tentar acessar `localhost:8080` e o Airflow não responder.

### 1. Executar o Docker como Administrador

[![Executar Docker como Administrador](https://github.com/JosiTubaroski/Subir_Docker/raw/main/img/Subir_Docker.png)](https://github.com/JosiTubaroski/Subir_Docker/blob/main/img/Subir_Docker.png)

---

## Verificando se o Docker subiu

### 2. Apresentação do Docker

Com o Docker Desktop aberto, confirme que ele está rodando corretamente.

[![Apresentação do Docker](https://github.com/JosiTubaroski/Subir_Docker/raw/main/img/Apresentacao_Docker.png)](https://github.com/JosiTubaroski/Subir_Docker/blob/main/img/Apresentacao_Docker.png)

Verifique também se o container do Airflow aparece na lista.

[![Ver container do Airflow](https://github.com/JosiTubaroski/Subir_Docker/raw/main/img/Ver-Airflow.png)](https://github.com/JosiTubaroski/Subir_Docker/blob/main/img/Ver-Airflow.png)

---

## Confirmando que o ambiente está pronto

### 3. Verificar pelo terminal

No `cmd`, dentro da pasta do projeto, digite:

```bash
docker-compose ps
```

[![Executando docker-compose ps](https://github.com/JosiTubaroski/Subir_Docker/raw/main/img/Executar_compose.png)](https://github.com/JosiTubaroski/Subir_Docker/blob/main/img/Executar_compose.png)

Se os containers aparecerem com status `Up`, o ambiente está pronto — basta acessar `localhost:8080` normalmente.

➡️ **Próximo passo:** [Conhecendo o Airflow](https://github.com/JosiTubaroski/Conhecendo_Airflow)
