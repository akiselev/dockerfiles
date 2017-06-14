FROM python:3.6

RUN apt-get update -qq
RUN apt-get install -qq apt-utils
RUN apt-get install -qq gfortran libatlas-base-dev
RUN apt-get install -qq pandoc

RUN pip install -U numpy tinysegmenter sumy
RUN python -c "import nltk; nltk.download('punkt')"

ENTRYPOINT ["sumy"]
CMD ["--help"]