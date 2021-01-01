FROM nanticj/pyenv

RUN pyenv install 3.9.1 && \
  pyenv global 3.9.1 && \
  python -m pip install --upgrade pip && \
  pip install --upgrade setuptools && \
  pip install wheel && \
  curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -

CMD bash
