# How to reduce the size of a docker image?

# 1. Use multistage build

# STAGE 1
FROM <base_image > AS builder

RUN 
COPY
RUN

# STAGE 2

FROM <base_image> AS 