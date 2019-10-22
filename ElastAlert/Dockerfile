FROM a1exeymatveev/elastalert:1.0
COPY config.yaml /usr/lib/elastalert/
COPY frequency.yaml /usr/lib/elastalert/example_rules
CMD cd /usr/lib/elastalert/ && elastalert-create-index && cd ~ && elastalert --config /usr/lib/elastalert/config.yaml  --rule example_rules/frequency.yaml
ENV TZ=Europe/Moscow     #Test