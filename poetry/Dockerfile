FROM nanticj/pyenv:1.2.27

RUN pyenv install 3.9.4 && \
  pyenv global 3.9.4 && \
  python -m pip install --upgrade pip && \
  pip install --upgrade setuptools && \
  pip install wheel && \
  curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -

CMD bash
