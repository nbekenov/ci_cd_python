# ci_cd_python
Continuous Integration With Python

virtualenv -p /usr/local/bin/python3.7 .env
source .env/bin/activate
pip install -r requirements.txt
flake8 --exclude=.env  --statistics
python -m pytest -v --cov=my_func
