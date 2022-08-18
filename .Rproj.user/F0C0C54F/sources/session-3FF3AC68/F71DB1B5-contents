# Practicing reprex

### NOT A REPREX
library(tidyverse)
library(palmerpenguins)

penguins |> 
  select(species, body_mass_g, flipper_length_mm, year) |> 
  filter(species == "Chinstrap") |> 
  str_to_lower(species) |> 
  group_by(islands) |> 
  summarize(mean(body_mass_g, na.rm = TRUE),
            mean(flipper_length_mm, na.rm =TRUE))

### A REPREX
library(tidyverse)

warpbreaks |> 
  str_to_lower(wool)

### A FIXING REPREX
library(tidyverse)

warpbreaks |> 
  mutate(wool = str_to_lower(wool))

### A REPREX WITH A SYNTHESIZE DATA FRAME
library(tidyverse)

wool_solution <- tribble(
  ~breaks, ~wool, ~tension,
  26, "A", "L",
  30, "A", "L,",
  54, "A", "L,",
  25, "A", "L,",
  70, "A", "L,"
)

wool_solution |> 
  mutate(wool = str_to_lower(wool))