---
title: R en marckdown
layout: 		post
comments:		false
tags: 
  - rusersgroup
noToc:			true
---
## Example of displaying htmlwidgets on a Github pages site

```{r}
library(plotly)
p <- ggplot(data = diamonds, aes(x = cut, fill = clarity)) +
            geom_bar(position = "dodge")
ggplotly(p)
```
