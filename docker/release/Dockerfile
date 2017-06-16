FROM rodrigocmn/todobackend-base:latest
MAINTAINER Rodrigo Nascimento <rodrigocmn@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse