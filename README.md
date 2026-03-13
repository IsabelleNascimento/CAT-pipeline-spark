# CAT-pipeline-spark
Estudos de Apache Spark com dataset CAT
Perfeito, Isabelle! Um **README.md** no GitHub serve para explicar o que é seu repositório, como rodar o código e o que você aprendeu. Como seu trabalho é um estudo, podemos deixar claro que é um **pipeline de aprendizado com Spark no Colab**, sem vender como projeto de produção.  

Aqui vai um modelo detalhado para você usar:

---

# CAT Pipeline com Apache Spark

Este repositório contém um **script de estudo** desenvolvido em **Google Colab** para explorar conceitos de **Apache Spark** aplicados ao dataset de **Comunicação de Acidente de Trabalho (CAT)**.

## 🎯 Objetivo
- Praticar leitura de dados com Spark.  
- Explorar tratamento de valores nulos.  
- Renomear colunas para evitar erros de execução.  
- Salvar dados em **Parquet particionado** (por UF e município).  
- Estruturar o código em formato executável via `spark-submit`.

## 📂 Estrutura
- `cat_pipeline.py` → Script principal com o pipeline Spark.  
- `README.md` → Este documento explicativo.  

## 🚀 Passos do Pipeline
1. **Leitura do CSV** com schema tipado.  
2. **Substituição de valores vazios** por `NULL`.  
3. **Renomeação automática de colunas** (remoção de espaços e caracteres especiais).  
4. **Tratamento de nulos em colunas de data** com valores default (`1900-01-01`).  
5. **Gravação em Parquet particionado** por `UF_Munic_Acidente`.  

## ▶️ Como executar
No ambiente Colab:
```bash
!python3 cat_pipeline.py
```

Em um ambiente com Spark instalado:
```bash
spark-submit cat_pipeline.py
```

## 📌 Observações
- Este trabalho foi desenvolvido em **Google Colab** apenas para fins de estudo.  
- O uso de Spark em Colab tem limitações, mas foi suficiente para compreender conceitos fundamentais como **particionamento** e **Parquet**.  
- Próximo passo: rodar o pipeline em um ambiente configurado com Spark local ou em cluster.  



