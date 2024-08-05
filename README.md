# Análise da extração mensal de petróleo nos estados do Nordeste:

A indústria petrolífera desempenha um papel importante na economia global, e o Brasil se destaca como um dos principais produtores de petróleo do mundo. Dentro do Brasil, a região Nordeste contribui significativamente para a produção nacional de petróleo. Este estudo se concentra na análise da produtividade de petróleo extraído maritimamente das plataformas dos estados do Nordeste do Brasil entre os anos de 2022 e 2024.

A análise da extração mensal de petróleo nesses estados é fundamental para entender a eficiência das operações, identificar padrões de produtividade e tomar decisões estratégicas informadas. Este trabalho visa responder a questões de negócio essenciais para gestores, economistas e engenheiros envolvidos na indústria petrolífera.

# Objetivos:

O objetivo deste estudo é responder às seguintes questões de negócio:

1) Qual é a produção total de óleo extraído em mar de cada estado do Nordeste entre 2022 e 2024?
2) Qual é a média, desvio padrão, mínimo e máximo da produtividade mensal de óleo de cada estado ao longo desses anos?
3) Existe alguma diferença significativa nas médias de produção de óleo/mês durante períodos produtivos entre os estados? Se houver, entre quais estados essas diferenças são observadas?
   
Este trabalho utilizará dados de produção de datasets públicos disponibilizados pela ANP (Agência Nacional do Petróleo) para realizar uma análise detalhada e fornecer insights sobre a extração de petróleo na região Nordeste do Brasil.

Arquivo da análise disponível nesse repositório em formato .ipynb em (Jupyter Notebook).

 # Desenvolvimento:
O primeiro problema de negócio foi resolvido estruturando o DataFrame coletado com as variáveis de interesse e agrupando a soma do total de óleo produzido (m³) por estado. Os resultados mostraram que Sergipe é o maior produtor de óleo da região Nordeste, seguido por Rio Grande do Norte e Bahia. Não houve registros de extração marítima de petróleo nos demais estados do Nordeste.

![output](https://github.com/user-attachments/assets/8e8415bf-f237-4448-807e-a9e4ea70ca39)

Para o segundo problema de negócio, os dados de estatística descritiva pertinentes (média, desvio padrão, mínimo e máximo) foram agrupados entre os estados, como mostrado na Figura à seguir: 

![estatistica_descritiva_produtividade](https://github.com/user-attachments/assets/569484c2-728f-492d-a7fb-1ff6ad4608b4)

Para resolver o terceiro problema de negócio, foi aplicado um teste ANOVA para verificar se pelo menos um dos estados se diferenciava significativamente em termos de produtividade mensal de óleo. Como mostrado na figura a seguir, o teste ANOVA revelou um p-valor muito inferior a 0,05, considerando um nível de significância de 5%. Isso indica que, de fato, existe pelo menos um estado com produtividade mensal de óleo significativamente diferente dos demais.

![ANOVA](https://github.com/user-attachments/assets/64fb4bba-5c2d-4dcd-b6ef-75796bc4cf30)

Para a verificação da significância entre pares, foi utilizado o Teste de Tukey. Os resultados do teste mostraram que não há uma diferença significativa na produtividade mensal entre os estados da Bahia e Rio Grande do Norte. No entanto, Sergipe se destacou com uma produtividade significativamente maior do que os demais estados.

![Tukey Test](https://github.com/user-attachments/assets/395c3e21-45ec-4a0d-9be5-e6324620661f)


# Conclusão:

Este estudo analisou a produtividade de petróleo extraído maritimamente nos estados do Nordeste do Brasil entre 2022 e 2024. A análise revelou que Sergipe é o maior produtor, seguido por Rio Grande do Norte e Bahia, com ausência de registros em outros estados da região.

O teste ANOVA indicou diferenças significativas na produtividade mensal entre os estados, e o Teste de Tukey confirmou que Sergipe se destaca com uma produtividade significativamente maior do que os demais estados, enquanto Bahia e Rio Grande do Norte não apresentam diferenças significativas entre si.

Esses resultados são importantes para a alocação eficiente de recursos e a formulação de estratégias para otimizar a produção.
