# \# ST606 Dissertation - Irish Mammal Sightings and Weather

### 

### \*\*Author:\*\* Kessiya Mary Jose (25250360)

### \*\*Supervisor:\*\* Dr Rafael De Andrade Moral

### \*\*Programme:\*\* MSc Data Science \& Analytics, Maynooth University

### \*\*Year:\*\* 2026

### 

### \## Project Overview

### 

##### This project investigates whether monthly weather conditions (temperature and rainfall) affect mammal sightings in Ireland using Bayesian hierarchical models.

### 

### \*\*Species studied:\*\*

##### \- Irish Hare (\*Lepus timidus subsp. hibernicus\*)

##### \- Red Fox (\*Vulpes vulpes\*)

##### \- Pine Marten (\*Martes martes\*)

### 

### \*\*Data sources:\*\*

##### \- Biodiversity Ireland - Mammals of Ireland 2016–2025 (NBDC)

##### \- Met Éireann weather data via CSO PxStat

### 

### \## Repository Structure

##### 

##### | File | Description |

##### |------|-------------|

##### | 1. Data Cleaning \& Preparation.Rmd | Initial data cleaning - 2 stations |

##### | 2. Expanded Data Cleaning.Rmd | Full cleaning - 9 stations, 15 counties |

##### | 3. EDA plots.Rmd | Exploratory data analysis - 8 plots |

##### | 4. Expanded Weather Variables.Rmd | Weather data expansion to 2023 |

##### | 5. JAGS Modelling.Rmd | Truncated Poisson models in JAGS |

##### | 6. Combined Model Results.Rmd | Combined temperature + rainfall + seasonal model |

##### | 7. Diagnostics.Rmd | PPC, prior-posterior overlap, negative binomial |

##### | 8. Additional Plots.Rmd | 3D plots and additional visualisations |

##### 

### \## Model

### 

##### Truncated Poisson hierarchical model fitted in JAGS:

### 

##### **Y\_ts \~ Poisson+(μ\_ts)**

### 

##### **log(μ\_ts) = (β₀ + b₀s) + (β₁ + b₁s)·temp +** **(β₂ + b₂s)·temp² + β₃·rainfall + α\[month]**

### 

### \## Requirements

##### 

##### \- R 4.5.2 or later

##### \- JAGS 4.3.1 or later

##### \- R packages: tidyverse, rjags, coda, patchwork, plotly, lubridate





### \## Copyright

###### 

###### © 2026 Kessiya Mary Jose. All rights reserved.

###### 

###### This repository contains dissertation work submitted for ST606 at Maynooth University. The code and analysis may be viewed for academic reference but may not be reproduced, copied or submitted as your own work without permission from the author.

###### 

###### Supervisor: Dr Rafael De Andrade Moral

###### Maynooth University, 2026

