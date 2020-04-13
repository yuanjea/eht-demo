FROM eventhorizontelescope/img-env

COPY eht-imaging/eht-imaging_pipeline.py /usr/local/src/
COPY wrapper.sh /usr/bin

WORKDIR /img
ENTRYPOINT ["/usr/bin/wrapper.sh"]
