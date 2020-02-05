FROM rabbitmq:3.8-alpine

RUN rabbitmq-plugins enable rabbitmq_event_exchange \
    && rabbitmq-plugins enable rabbitmq_amqp1_0 \
    && rabbitmq-plugins enable rabbitmq_management \
    && rabbitmq-plugins enable rabbitmq_stomp \
    && rabbitmq-plugins enable rabbitmq_web_stomp
