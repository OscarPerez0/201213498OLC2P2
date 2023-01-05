FROM python:3.9

EXPOSE 8501

WORKDIR /app

COPY  requirements.txt ./requirements.txt
RUN pip install -r requirements.txt
RUN pip install streamlit
RUN pip install pandas
RUN pip install xlrd
RUN pip install matplotlib
RUN pip install numpy
RUN pip install -U scikit-learn
RUN pip install scikit-metrics

RUN git clone https://github.com/OscarPerez0/201213498OLC2P2.git

RUN pip install -r requirements.txt

ENTRYPOINT ["streamlit", "run", "./201213498OLC2P2/app/Home.py", "--server.port=8501", "--server.address=0.0.0.0"]