### 🎯 Projeto: Plataforma de Monitoramento de Tráfego de Aplicações Web

#### 🔧 Tecnologias:
- **Apache Spark / PySpark**
- **Delta Lake** (com features como Time Travel, Vacuum, Constraints, etc.)
- **Databricks Community Edition** ou Spark local
- **Apache Kafka** (para ingestão em streaming, opcional)
- **Apache Airflow** ou **Databricks Jobs** para orquestração

#### 🧱 Arquitetura Medallion:
1. **Bronze Layer**: Dados brutos (logs JSON, CSV ou via Kafka)
2. **Silver Layer**: Dados limpos e normalizados
3. **Gold Layer**: Métricas analíticas agregadas (KPIs de uso)

#### 💡 Funcionalidades a Demonstrar:
- Leitura de dados em *streaming* e *batch*
- Transformações com Delta Lake e PySpark
- Uso de `MERGE`, `UPDATE`, `DELETE` para deduplicação e correções
- Particionamento e `OPTIMIZE ZORDER` para performance
- Time Travel e RESTORE de versões
- Monitoramento da tabela com `DESCRIBE HISTORY` e metadados
- Governança com constraints e schema evolution
- (Opcional) Data Sharing com Delta Sharing

#### 📊 Métricas Exemplares:
- Número de requisições por IP por dia
- Taxa de erros por endpoint
- Duração média de sessões por usuário