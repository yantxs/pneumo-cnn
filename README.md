# Pneumo CNN 
![](https://img.shields.io/github/license/yantxs/pneumo-cnn)
### _Classificação de pneumonia via radiografia de tórax_


Repositório referente aos trabalhos desenvolvidos durante o ciclo do PIBIC 2020/21 orientado pela Prof.ª Drª. Karin Komati. 
   * [Sobre](#Sobre)
   * [Tecnologias](#tecnologias)
   * [Dataset](#dataset)
   * [Rede Neural Convolucional](#rede-neural-convolucional)
      * [O que são Rede Neurais Convolucionais?](#o-que-sao-rede-neurais-convolucionais)
   * [Estrutura de diretório](#testes)
   * [Licencas](#tecnologias)

#### Sobre
Pneumonia é uma doença caracterizada pela inflamação dos pulmões, e o seu diagnóstico é realizado com base nos sintomas, exame físico, análise bioquímica, análise microbiológica e radiológico, sendo geralmente a radiografia de tórax que é um elemento-chave no diagnóstico. 

Usualmente, médicos analisam padrões radiológicos específicos associados a dados clínicos e laboratoriais para diferenciar a pneumonia entre etiologia viral e bacteriana. Radiografias que apresentam doença localizada com consolidações geralmente indicam uma infecção por bactérias, entretanto, exames que apresentam um padrão intersticial ou espessamento peribrôquico tendem a ser uma infecção de origem viral. 

Desta forma o presente trabalho se compromete em estudar, implementar e analisar o uso de redes neurais convolucionais no auxilio do diagnóstico e classificação da pneumonia através de imagens de raio-X.
#### Tecnologias

Foram utilizadas algumas ferramentas e tecnologias para o desenvolvimento deste trabalho, dentre elas:

- [Python] - linguagem de programação de alto nível, interpretada de script, imperativa, orientada a objetos, funcional, de tipagem dinâmica e forte.
- [Jupyter Notebook] - ferramenta de Literate Computing, simples e extremamente eficientes, pois permite unir código e texto.
- [TensorFlow] - biblioteca de código aberto para aprendizado de máquina aplicável a uma ampla variedade de tarefas.
- [Keras] - biblioteca de rede neural de código aberto escrita em Python.
- [Collab] - ambiente de notebooks Jupyter que não requer configuração e é executado na nuvem, disponibilizado pelo Google.


#### Dataset

A base de dados utilizada foi a Chest X-Ray Images (Pneumonia) disponibilizada de forma pública na plataforma [Kaggle].


Essa base de dados contém 5,863 imagens de radiografia de tórax de criancças de 1 a 5 anos.

#### Rede Neural Convolucional
Neste repositório existe 4 modelos diferentes de Rede Neural Convolucional para resolução do problema proposto neste trabalho. 
##### O que são Rede Neurais Convolucionais?

Uma rede neural convolucional é um tipo especial de implementação de inteligência artificial que utiliza de manipulações matemáticas de matrizes para processar imagens. 

- Uma **convolução** é dada pela multiplicação de uma matriz por outra, sendo gerada uma terceira
- A rede recebe uma imagem de entrada e usa um filtro (*ou kernel*) para criar o mapa de caracteristas (*feature map*) descrevendo a imagem
- Na operação de convolução nós pegamos um filtro (*usualmente 2x2 or 3x3*) e percorremos sobre a matriz da imagem. Os números são multiplicados e é gerado um produto que descreve esse espaço da matriz gerada da imagem maior. Esse processo é repetido sobe toda a imagem, como pode ser visto na animação abaixo:

![gif](https://cdn-images-1.medium.com/max/800/1*VVvdh-BUKFh2pwDD0kPeRA@2x.gif)

> Abaixo uma representação 2D do que está acontecendo em 3 dimensões, utilizando um filtro 3x3.

![img](https://cdn-images-1.medium.com/max/800/1*EuSjHyyDRPAQUdKCKLTgIQ.png)

- Usamos diferentes filtros para passer sobre nossa entrada, extraímos todos os mapas de caracteristicas, agrupamos e colocamos como a saída da camada convolucional.
- E então passamos o resultado dessa saída por uma função de ativação


#### Estrutura de diretório

O repositório está organizado da seguinte maneira:

| Arquivo | Descrição |
| ------ | ------ |
| [src/model1/index.ipynb][model1] | Notebook com o modelo 1 de RNC proposto para classificação binária entre pneumonia ou normal. |
| [src/model2/index.ipynb][model2] | Notebook com o modelo 2 de RNC proposto para classificação binária entre pneumonia ou normal. |
| [src/model3/index.ipynb][model3] | Notebook com o modelo 3 de RNC proposto para classificação multiclasse entre normal, pneumonia viral e bacteriana. |
| [src/model4/index.ipynb][model4] | Notebook com o modelo 4 de RNC proposto para classificação multiclasse entre normal, pneumonia viral e bacteriana. |



## Licença

MIT

Yan **Teixeira**
    
   [Python]: <https://python.org>
   [Jupyter Notebook]: <https://jupyter.org/>
   [TensorFlow]: <https://www.tensorflow.org/>
   [Keras]: <https://keras.io/>
   [Collab]: <https://colab.research.google.com/>
   [Kaggle]: <https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia>
   [model1]: <https://github.com/yantxs/pneumo-cnn/blob/main/model1/index.ipynb>
   [model2]: <https://github.com/yantxs/pneumo-cnn/blob/main/model2/index.ipynb>
   [model3]: <https://github.com/yantxs/pneumo-cnn/blob/main/model3/index.ipynb>
   [model4]: <https://github.com/yantxs/pneumo-cnn/blob/main/model4/index.ipynb>
   
