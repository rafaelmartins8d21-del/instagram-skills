---
name: ig-analise-videos
description: "Analisa métricas e retenção dos vídeos do Rafa Martini (Instagram, TikTok, YouTube Shorts) e diz o que resulta melhor e pior, com decisões concretas. Usar com prints de Insights, CSV ou Postiz."
---

# Análise de Vídeos — RAFA MARTINI

O objetivo é decidir o que fazer a seguir, não despejar números. Cada análise acaba em decisões concretas: fazer mais, fazer menos, testar.

Lê primeiro `../../references/voice-profile.md` para saber quem é o Rafa e o público dele. Responde sempre em português de Portugal, informal e direto.

## 1. Recolher os dados

Usa a fonte que houver, por esta ordem:

1. **Prints dos Insights (a melhor fonte para retenção).** O gráfico de retenção só existe dentro das apps. Pede ao Rafa, por vídeo:
   - Instagram: visualizações, alcance, tempo médio de visualização, gráfico de retenção, taxa de skip (se aparecer), partilhas, guardados, gostos, comentários, seguidores ganhos, % não-seguidores.
   - TikTok: visualizações, tempo médio, % que viu o vídeo completo, gráfico de retenção, partilhas, guardados, seguidores ganhos, origem do tráfego (For You vs perfil).
   - YouTube Shorts: visualizações, % "viram vs passaram à frente", duração média, retenção, subscritores ganhos.
2. **Postiz** (se estiver ligado): `postiz analytics:post <post-id> -d 30` para os números. O Postiz não dá curvas de retenção, por isso a retenção continua a vir dos prints.
3. **CSV ou export** que o Rafa enviar.

Para cada vídeo precisas também de:
- duração do vídeo em segundos
- data e hora de publicação
- se foi Trial Reel ou publicação direta
- o vídeo em si ou uma descrição dos primeiros 3 segundos

Se faltar alguma coisa, pede só o que falta. Nunca inventes nem estimes números: um campo sem dados fica `[em falta]`.

## 2. Etiquetar cada vídeo

Dá a cada vídeo estas etiquetas (confirma-as com o Rafa na primeira vez):
- **Formato:** mashup, cover, original, bastidores/estúdio, humor/sketch, trend, a atuar para desconhecidos, parceria (ex.: Sumol)
- **Tipo de hook:** a meio da ação, pergunta, texto provocador no ecrã, a primeira nota a cantar, humor
- **Duração:** até 15 s, 15-30 s, 30-60 s, mais de 60 s
- **Plataforma**

## 3. Calcular as métricas

Por vídeo:
- **Retenção média** = tempo médio ÷ duração
- **Hold do hook** = % que ainda está a ver aos 3 s (lido do gráfico)
- **Onde cai:** o segundo em que a curva tem a maior descida. Vê o que acontece no vídeo nesse momento.
- **Partilhas por 1.000 de alcance** (o sinal mais forte no Instagram)
- **Guardados por 1.000 de alcance**
- **Seguidores por 1.000 de alcance** (conversão em fãs)
- **Comentários por 1.000 de alcance**
- **% não-seguidores** (quanto o vídeo saiu da bolha)

**Compara sempre com a mediana dos vídeos do próprio Rafa**, não com médias genéricas da internet. Cada vídeo fica marcado como acima, na média ou abaixo da mediana dele, métrica a métrica.

## 4. Manter o registo

Guarda cada vídeo analisado num registo (folha de cálculo) com as colunas: data, plataforma, formato, hook, duração, visualizações, alcance, retenção média, hold aos 3 s, segundo da maior queda, partilhas/1k, guardados/1k, seguidores/1k, comentários/1k, % não-seguidores, Trial Reel (s/n), notas.

Se o Rafa já tiver um registo, acrescenta-lhe as linhas novas. Se não tiver, cria um e pergunta onde o quer guardar.

## 5. Encontrar padrões

Com o registo todo, compara por formato, tipo de hook, duração, plataforma e hora de publicação.

Regras:
- **Com menos de 5 vídeos num grupo**, diz que é só uma pista, não uma conclusão.
- **Separa alcance de ligação:** um vídeo com muitas visualizações e poucos seguidores ganhos não é necessariamente um vencedor. Para o crescimento do artista contam mais as partilhas e os seguidores ganhos.
- **Retenção baixa com hook forte** quer dizer que o problema está no meio do vídeo, não na abertura. Aponta o segundo exato.
- Se um Trial Reel correu bem, sugere repetir o formato com publicação direta.
- Quando a análise aponta para um hook ou legenda nova, passa a ideia ao `ig-caption-writer` ou ao `ig-hook-extractor`.

## 6. Entregar

Formato da resposta, curto e para ler no telemóvel:

1. **Resumo numa linha:** o que está a resultar agora.
2. **Top 3 e bottom 3** vídeos, cada um com uma linha a dizer porquê (a métrica e o momento do vídeo).
3. **Onde as pessoas saem:** os padrões de queda (ex.: "nos mashups perdes 40% na passagem para a segunda música").
4. **Decisões:**
   - Fazer mais: …
   - Fazer menos ou parar: …
   - Testar a seguir (de preferência como Trial Reel): …
5. **Dados em falta** que melhorariam a próxima análise.

Se o Rafa pedir um documento para mostrar ao manager, faz a mesma estrutura em PDF ou PPTX, com espaços `[por preencher]` onde faltarem valores.
