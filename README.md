# first-sim4
just test# Install & load packages
packages <- c("ggplot2", "dplyr")
lapply(packages, function(p) if (!require(p, character.only = TRUE)) install.packages(p))

library(ggplot2)
library(dplyr)

# ---- Simulate sequential blood pressure readings ----
set.seed(2025)
days <- 1:30
patients <- paste0("Patient_", 1:5)

data <- expand.grid(Day = days, Patient = patients)
data$SystolicBP <- rnorm(nrow(data), mean = 120, sd = 10)

# Introduce some trend/anomalies
data$SystolicBP[data$Patient == "Patient_3" & data_]()

