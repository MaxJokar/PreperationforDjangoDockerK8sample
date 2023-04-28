FROM python:3.10-buster

COPY . /app
WORKDIR /app

RUN python -m venv /opt/venv

# RUN pip install pip --upgrade
# RUN /opt/venv/bin/pip install -r requirements.txt
# RUN chmod +x entrypoint.sh

# installing things & run
RUN /opt/venv/bin/pip install pip --upgrade && \
    /opt/venv/bin/pip install -r requirements.txt && \
    chmod +x entrypoint.sh



CMD ["/app/entrypoint.sh"]