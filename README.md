# llm-assistant

1. 创建虚拟环境并安装依赖
    ```bash
    conda create -n llm_env python=3.11
    conda activate llm_env
    pip install -r requirements.txt
    ```
2. 配置环境变量
    打开`.env.example`文件
    填写完整该文件中的`OPENAI_API_KEY`、`HTTP_PROXY`、`HTTPS_PROXY`三个环境变量
    把`.env.example`文件重命名为`.env`
3. docker运行qdtant容器

    ```bash
    docker pull qdrant/qdrant
    docker run -p 6333:6333 qdrant/qdrant
    ```

4. 运行app.py文件