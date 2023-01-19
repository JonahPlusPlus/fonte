# Installation
1. Install Python 3.9 on your machine
  - If using `pyenv`, use these commands:

    ```
    pyenv install 3.9.1
    pyenv local 3.9.1
    ```
2. Install the required Python packages
    ```
    python -m pip install numpy==1.21.0 pandas==1.4.3 scipy==1.9.0 tqdm matplotlib==3.4.0 seaborn==0.11.1 rank-bm25==0.2.2 tabulate==0.8.9 jupyter setuptools
    python -m pip install lib/SBFL
    python -m pip install lib/spiral
    ```

3. Check the installation by running Fonte using this sample command:
    ```bash
    python Fonte.py data/Defects4J/core/Cli-29b -o output.csv
    # Number of total commits: 616
    #          vote  rank  is_style_change
    # commit
    # c0d5c79   1.0   1.0            False
    # 147df44   0.0   2.0             True
    ```
 
4. Download the [Docker client](https://www.docker.com/products/docker-desktop/) (only needed for replication or extension) and run the Docker daemon

5. Check the docker installation by running these commands:
    ```bash
    docker pull agb94/fonte:latest
    ```