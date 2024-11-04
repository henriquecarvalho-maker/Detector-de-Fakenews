<h1>Detector de Fake News</h1>

<p>Este repositório contém um projeto de <strong>Detector de Fake News</strong>, cujo objetivo é desenvolver um modelo de aprendizado de máquina capaz de classificar notícias como reais ou falsas. A ideia é auxiliar na identificação de desinformação, proporcionando uma ferramenta prática para análise automática de conteúdo.</p>

<h2>Sumário</h2>
<ul>
    <li><a href="#descrição-do-projeto">Descrição do Projeto</a></li>
    <li><a href="#instalação">Instalação</a></li>
    <li><a href="#como-usar">Como Usar</a></li>
    <li><a href="#estrutura-do-projeto">Estrutura do Projeto</a></li>
    <li><a href="#resultados">Resultados</a></li>
    <li><a href="#tecnologias-utilizadas">Tecnologias Utilizadas</a></li>
    <li><a href="#contribuição">Contribuição</a></li>
    <li><a href="#licença">Licença</a></li>
</ul>

<h2 id="descrição-do-projeto">Descrição do Projeto</h2>
<p>O <strong>Detector de Fake News</strong> utiliza um modelo de <strong>Regressão Logística</strong> para realizar a classificação binária entre notícias reais e falsas. Com uma precisão de cerca de 98% no conjunto de testes, o modelo foi avaliado e ajustado com técnicas de <strong>validação cruzada</strong> para garantir sua generalização e minimizar o overfitting. Este projeto pode ser expandido para utilizar outros algoritmos e técnicas de NLP.</p>

<h2 id="instalação">Instalação</h2>
<ol>
    <li><strong>Clone o repositório:</strong>
        <pre><code>git clone https://github.com/henriquecarvalho-maker/Detector-de-Fakenews.git</code></pre>
    </li>
    <li><strong>Crie um ambiente virtual</strong> (opcional, mas recomendado):
        <pre><code>python -m venv env 
source env/bin/activate  # Linux/Mac 
.\env\Scripts\activate   # Windows</code></pre>
    </li>
    <li><strong>Instale as dependências</strong>:
        <pre><code>pip install -r requirements.txt</code></pre>
    </li>
</ol>

<h2 id="como-usar">Como Usar</h2>
<ol>
    <li><strong>Preparação do Dataset:</strong> Coloque seu dataset na pasta <code>dados/</code>. O projeto foi originalmente baseado no dataset de Fake News Detection no Kaggle, estruturado com colunas como <code>title</code>, <code>text</code>, <code>date</code>, <code>category</code>, <code>subcategory</code>, e <code>link</code>.</li>
    <li><strong>Pré-processamento:</strong> Execute o notebook de pré-processamento para limpar e preparar os dados para a modelagem.</li>
    <li><strong>Treinamento do Modelo:</strong> No notebook principal, execute as células para treinar e avaliar o modelo de classificação. O notebook inclui métricas de desempenho, como precisão, recall e F1-score.</li>
    <li><strong>Testar com Novos Dados:</strong> Para testar novas amostras, execute o notebook fornecendo a entrada de texto e observe a classificação.</li>
</ol>

<h2 id="estrutura-do-projeto">Estrutura do Projeto</h2>
<ul>
    <li><code>dados/</code>: Contém o dataset utilizado para o treinamento e validação do modelo.</li>
    <li><code>Analise_exploratoria.ipynb/</code>: Notebooks Jupyter com análise exploratória e pré-processamento dos dados do modelo.</li>
    <li><code>classificador_texto.ipynb/</code>: Manipulação de dados e funções para o modelo.</li>
    <li><code>requirements.txt</code>: Arquivo com as dependências do projeto.</li>
</ul>

<h2 id="resultados">Resultados</h2>
<p>O modelo alcançou uma precisão média de <strong>98.76%</strong> na validação cruzada (com variação entre 98.58% e 98.95%) e apresentou uma precisão de cerca de <strong>99.01%</strong> no conjunto de testes. Mesmo com alta acurácia, observou-se sinais de overfitting, o que pode ser aprimorado em versões futuras do projeto. <strong>Possivelmente o modelo carece de mais dados para melhor aprendizado e, portanto melhor generalização.</strong></p>

<h2 id="tecnologias-utilizadas">Tecnologias Utilizadas</h2>
<ul>
    <li><strong>Linguagem:</strong> Python</li>
    <li><strong>Bibliotecas principais:</strong>
        <ul>
            <li>Pandas e NumPy para manipulação de dados</li>
            <li>Scikit-Learn para modelagem e validação</li>
            <li>NLTK ou spaCy para processamento de linguagem natural</li>
        </ul>
    </li>
</ul>

<h2 id="contribuição">Contribuição</h2>
<p>Contribuições são bem-vindas! Para contribuir:</p>
<ol>
    <li>Realize um fork do repositório.</li>
    <li>Crie uma branch para sua contribuição:
        <pre><code>git checkout -b feature/nome-da-feature</code></pre>
    </li>
    <li>Commit suas alterações e faça um push:
        <pre><code>git push origin feature/nome-da-feature</code></pre>
    </li>
    <li>Crie um Pull Request com uma descrição do que foi modificado.</li>
</ol>

<h2 id="licença">Licença</h2>
<p>Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.</p>
