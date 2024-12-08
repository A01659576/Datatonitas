# Datatonitas
Proyecto que facilita la detección y sanción de posibles actos de colusión.

#Integrantes
América Andrea Espinoza Sánchez
Ana Paola Villanueva Medrano
Allison Marianne Zepeda Beltrán
Paulina Leal Mosqueda
Fernanda Leal Mosqueda

#¿Qué hace el proyecto?
El proyecto es una herramienta que utiliza datos del sistema 6 de la Plataforma Digital Nacional (PDN). El código observa la diferencia porcentual entre el presupuesto para licitaciones y el valor de los contratos otorgados. Para ello, se toma en cuenta el porcentaje establecido por el Banco Mundial, el cual establece que si la diferencia es mayor o igual al 30%, significa que hay un posible acto de colusión (Kenny & Musatova, 2010). Asimismo, el código detecta si el plazo del tiempo entre la publicación de la licitación y el cierre es menor a 15 días conforme a lo indicado por la Ley de Adquisiciones, Arrendamientos y Servicios del Sector Público (LAASSP, 2021) en su artículo 32. En este sentido, busca detectar posibles actos de corrupción en los procesos de contrataciones relacionados con colusión y, en su caso, que haya una sanción.

Por otro lado, el código se realizó utilizando Python y las librerías usadas son: polars, json, re, dateutil.parser, google.colab, IPython.display y ipywidgets. Adicionalmente, las variables utilizadas fueron el ID de la contratación, entidad federativa, el valor del tender (licitación), el monto del contrato, la descripción del contrato, fecha de inicio del tender y su fecha de terminación.

¿Por qué el proyecto es útil?
Permite combatir los actos de corrupción en los procesos de contratación, de forma que es un mecanismo que protege el Estado de derecho. Los red flags son indicadores que permitirán que en futuras investigaciones se pueda tener una delimitación de cuáles son los casos a observar para detectar situaciones de colusión. Igualmente, se le pueden añadir nuevas variables al código, si se desearé encontrar nueva información en un futuro. En este sentido, si se busca encontrar más cosas relacionadas con los indicadores que detecta el programa,  el futuro usuario podría hacer un cruce de datos con otros sistemas de la Plataforma Digital Nacional.

¿Cómo pueden comenzar los usuarios con el proyecto?
Los usuarios pueden utilizar la herramienta al subir los archivos json de la Plataforma Digital Nacional provenientes del sistema 6. Los archivos que se deben subir son únicamente los correspondientes a las entidades federativas. Una vez que se realicé este paso, se pueden utilizar los filtros correspondientes (por tipo de bandera, estado, ID y proveedor). Lo anterior, le permitirá al usuario acceder a la información que le sea de su interés. Por otra parte, en la parte superior de los filtros, se desplegará un conteo con el número de red y green flags, el cual se actualizará cada que se cambien los filtros.

Link del código en Google Colab: https://colab.research.google.com/drive/1VxveUcs3jDGNGa-hPwo2nVBtnXzCj4WU?usp=sharing

Para mayor información consultar artículo del Banco Mundial: https://openknowledge.worldbank.org/server/api/core/bitstreams/f70c333b-e7d3-5349-ad6a-ddb4865e5904/content

