FROM python:3.9
WORKDIR /app

RUN pip3 install 'git+https://github.com/AdamStrojek/libetrv.git' -r ./requirements.txt
COPY ./run.sh .
RUN chmod +x run.sh

ENTRYPOINT ["tail"]
CMD ["-f","/dev/null"]

#CMD ["/app/run.sh"]
