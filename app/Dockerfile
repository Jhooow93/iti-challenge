FROM gradle:4.10

RUN git clone https://github.com/itidigital/plataform-challenge.git \
    && chown -R gradle:gradle plataform-challenge

USER gradle
WORKDIR plataform-challenge/app

RUN gradle build

ENTRYPOINT ["gradle", "run"]