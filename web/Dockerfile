FROM python:3
WORKDIR /usr/src/app
COPY requirements.txt ./
COPY en_core_web_sm-3.0.0 ./
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
# RUN pip install --no-cache-dir --upgrade pip && \
# RUN pip install en_core_web_sm-2.1.0.tar.gz

CMD ["python", "app.py"]

# FROM python:3.9
#
# # WORKDIR /app
# WORKDIR /usr/src/app
#
# COPY requirements.txt ./
# COPY en_core_web_sm-2.1.0.tar.gz ./
#
# RUN python -m venv venv
# RUN . venv/bin/activate && pip install -r requirements.txt
# # RUN . venv/bin/activate && pip install en_core_web_sm-2.1.0.tar.gz
# # RUN . venv/bin/activate -m spacy download en_core_web_sm-2.1.0-py3.9.egg-info
# # COPY . .
#
# WORKDIR /usr/src/app
#
# CMD [ "venv/bin/python", "app.py" ]