# FIAP - SPRINT1_2CCA

## **1. Qual problema vocês escolheram resolver?**

- O processo atual de gestão de áreas verdes da Motiva é lento e oneroso. 
- Dependência de visitas semanais com coleta física de dados.  
- Processo manual sujeito a falhas e imprecisões de monitoramento.

**Quem é o usuário do app?**

- Operador de campo (equipe de manutenção e corte).
- Supervisor de operações.

**Qual é a principal ação do app?**

- Listar as áreas verdes que necessitam de intervenção, baseando-se no que foi identificado pelos drones e previsto pelo modelo XGBoost.
- Registrar a conclusão do corte ou reportar anomalias, retroalimentando o dataset do sistema de inteligência artificial em tempo real para otimizar futuras previsões.

## **2. Funcionalidades do app (MVP)**

- Listagem de ocorrências: Tela principal exibindo os setores de gramado organizados por prioridade de manutenção, conforme os mapas digitais gerados.  
- Visualização de detalhe: Acesso a informações específicas do trecho selecionado, como altura atual prevista pelo modelo (ex: 15cm)  e localização no mapa.  
- Cadastro de ocorrência / Confirmação: Botão para o operador confirmar que a grama foi cortada (atualizando o status do dataset) ou adicionar uma nova ocorrência manual com foto da câmera do celular.
- Classificação de risco: Indicadores visuais simples de prioridade (Baixa, Média, Alta) ditados pelas decisões baseadas em inteligência artificial.

## **3. Protótipo navegável (Figma ou outro a critério do grupo)**
- link do lovable: https://drone-vision-watch.lovable.app/
- link do repositório genérico: https://github.com/ferteama/drone-vision-watch.git
  #### Lembrando, o foco principal dessa demonstração no lovable é apenas o visual, não iremos assumir essa estrutura como arquitetado no repositório
## **4. Estrutura técnica do projeto**
```
  src/
   screens/
     HomeScreen.tsx
     DetailScreen.tsx
     FormScreen.tsx
   components/
     OcorrenciaCard.tsx
     Header.tsx
   types/
     index.d.ts
```
