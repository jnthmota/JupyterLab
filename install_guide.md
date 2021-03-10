# Instalação Recomendada (Windows)


## Miniconda

Acesse https://docs.conda.io/en/latest/miniconda.html e faça o dowload do instalador.

Execute o instalador.
Além da tradicional caixa de diálogo perguntando o caminho onde deseja realizar a instalação e se a instalação é pra todos os usuários, esse instalador vai dar a opção de adicionar o caminho ao PATH e de tornar o interpretador python dessa instalação como o padrão do sistema.
Recomendo não ticar nenhuma das caixas, assim como o instalador.

## Ambiente Virtual

Uma vez instalado é possível abrir tanto Anacoconda Command Prompt como Anacoconda Powershell, ao gosto do freguês.

Criação:

```powershell
conda create -n nome_do_ambiente_venv python
```

Ativação:

```powershell
conda activate nome_do_ambiente_venv
```

## Instalando pacotes com conda

```powershell
conda install -c conda-forge jupyterlab
conda install pandas
```

Deixei o comando de instalação do Jupyter Lab por 2 motivos.
Primeiro, pra mostrar que nem sempre a instalação de um pacote pelo conda será feita com `conda install nome_do_padote`.
Segundo, pra deixar a recomendação de usarem o Jupyter Lab.


## Abrindo Jupyter Lab

Simples assim:

```powershell
jupyter-lab
```

Ele abre e roda em algum navegador.
Acredito que funciona bem em Firefox (e talvez até no Edge), mas recomendo algum baseado em Chromium pra rodar já que é o foco dos desenvolvedores do projeto Jupyter.

# Instalação Recomendada (Ubuntu)

Distribuições Linux costumam já ter um interpretador python instalado.
Ubuntu, em particular vem com 2.
`python` é comando para python 2.7 e `python3` para python 3.6 (talvez 3.8 na última lts)

Então não precisa instalar python de lugar nenhum, só sair usando.
Mas ainda é recomendado criar ambientes virtuais antes de instalar pacotes

## Ambiente Virtual

Criação:

```bash
cd ~/caminho_do_projeto
python3 -m venv nome_do_ambiente_venv
```

Ativação:

```bash
source activate ~/caminho_do_projeto/bin/activate
```

## Instalando pacotes com pip

Com ambiente virtual ativado é só instalar tudo que quiser com `pip install`

```bash
pip install jupyterlab
pip install pandas
```

## Abrindo Jupyter Lab

Simples assim:

```bash
jupyterlab
```

Ele abre e roda em algum navegador.
Acredito que funciona bem em Firefox (e talvez até no Edge), mas recomendo algum baseado em Chromium pra rodar já que é o foco dos desenvolvedores do projeto Jupyter.