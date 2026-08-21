# Atividade Prática - Integração Contínua (CI)

## 1. Nome dos alunos:

- Breno Luiz da Silva Ferreira
- Caique Pinto da Costa

## 2. Repositório

Link: https://github.com/BrenoFerreira01/atividade-devops-ci

## 3. Ferramentas utilizadas

- Git
- GitHub
- GitHub Actions
- Python
- Pytest

## 4. O que foi desenvolvido?

Um módulo de operações matemáticas básico (soma, subtração e multiplicação), utilizando Python, em conjunto com testes unitários para validar o resultado dessas operações.

## 5. Como funciona a pipeline?

Toda vez que uma branch main é atualizda com o comando git push, a automação é ativada. O GitHub simula uma máquina Ubunto, configurando o ambiente python, baixando as dependências necessárias e executa os testes. Caso o calculo dê certo, aprovado, se não, o fluxo é interrompido.

## 6. Teste realizado

Desenvolveram-se três testes unitários para validar a assertividade de cada uma das funções (test_soma, test_subtracao e test_multiplicacao).

![ETAPA A](./img/ETAPA_A.png)

## 7. Falha proposital

Na etapa B, foi criado um erro proposital. Foi trocado o operador matemático da função de soma, tornando-a uma subtração.

![ETAPA B](/img/ETAPA B.png)

## 8. Resultado

O pipeline barrou o código. O GitHub Actions executou o Pytest, o assert se tornou falso, obrigando a pipeline a gerar um alerta vermelho.

![ETAPA C](/img/ETAPA C.png)

## 9. Conclusão

A Integração Contínua (CI) atua como um inspetor de qualidade automatizado. Em projetos acadêmicos mais densos, como o desenvolvimento de algoritmos complexos, é comum que a correção de um bloco de código acabe quebrando outro componente sem o desenvolvedor perceber. A CI impede que esse código com falhas integre a versão principal do projeto, detectando o erro de forma imediata antes que ele gere impactos maiores.
