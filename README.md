# Detecci-n-de-hongos-venenosos
Proyecto de ML para detectar hongos venenosos (y no recomendables), y no venenosos

Este proyecto emplea la base de datos de https://archive.ics.uci.edu/dataset/73/mushroom
Mushroom [Dataset]. (1981). UCI Machine Learning Repository. https://doi.org/10.24432/C5959T.

Este conjunto de datos incluye descripciones de muestras de 23 especies de hongos pertenecientes a las familias Agaricus y Lepiota. Cada especie está clasificada como comestible, venenosa o desconocida (y no recomendada). Para este problema se agruparon las no comestible con las no recomendadas.

No existe una regla para determinar si un hongo es comestible, es decir una sola característica no puede ser utilizada para determinar si es peligroso o no como en otras plantas venenosas como el roble o la hiedra venenosa.

Este dataset nos presenta un problema de clasificación binaria (venenoso o no venenoso) donde la variable objetivo "es poisonous". Todas las variables de este problema son categóricas, contando con 22 características y 1 variable objetivo. Como nota adicional sabemos que este dataset cuenta con valores faltantes en la columna "stalk-root".

Resumen de las variables proporcionado por UCI:
  1. cap-shape:                bell=b,conical=c,convex=x,flat=f, knobbed=k,sunken=s
  2. cap-surface:              fibrous=f,grooves=g,scaly=y,smooth=s
  3. cap-color:                brown=n,buff=b,cinnamon=c,gray=g,green=r, pink=p,purple=u,red=e,white=w,yellow=y
  4. bruises?:                 bruises=t,no=f
  5. odor:                     almond=a,anise=l,creosote=c,fishy=y,foul=f, musty=m,none=n,pungent=p,spicy=s
  6. gill-attachment:          attached=a,descending=d,free=f,notched=n
  7. gill-spacing:             close=c,crowded=w,distant=d
  8. gill-size:                broad=b,narrow=n
  9. gill-color:               black=k,brown=n,buff=b,chocolate=h,gray=g, green=r,orange=o,pink=p,purple=u,red=e, white=w,yellow=y
  10. stalk-shape:              enlarging=e,tapering=t
  11. stalk-root:               bulbous=b,club=c,cup=u,equal=e, rhizomorphs=z,rooted=r,missing=?
  12. stalk-surface-above-ring: fibrous=f,scaly=y,silky=k,smooth=s
  13. stalk-surface-below-ring: fibrous=f,scaly=y,silky=k,smooth=s
  14. stalk-color-above-ring:   brown=n,buff=b,cinnamon=c,gray=g,orange=o, pink=p,red=e,white=w,yellow=y
  15. stalk-color-below-ring:   brown=n,buff=b,cinnamon=c,gray=g,orange=o, pink=p,red=e,white=w,yellow=y
  16. veil-type:                partial=p,universal=u
  17. veil-color:               brown=n,orange=o,white=w,yellow=y
  18. ring-number:              none=n,one=o,two=t
  19. ring-type:                cobwebby=c,evanescent=e,flaring=f,large=l, none=n,pendant=p,sheathing=s,zone=z
  20. spore-print-color:        black=k,brown=n,buff=b,chocolate=h,green=r, orange=o,purple=u,white=w,yellow=y
  21. population:               abundant=a,clustered=c,numerous=n, scattered=s,several=v,solitary=y
  22. habitat:                  grasses=g,leaves=l,meadows=m,paths=p, urban=u,waste=w,woods=d
  23. poisonous:                edible=e, poisonous=p

