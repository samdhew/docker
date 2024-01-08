FROM amazoncorretto:17-alpine

# Install specific versions of curl and tzdata
RUN apk --no-cache add curl=8.3.0-r0 tzdata=2023c-r0

# Alternatively, to install the latest version
# RUN apk --no-cache add curl tzdata

# Set the timezone to America/New_York
ENV TZ="America/New_York"

# Display the current date
RUN date
