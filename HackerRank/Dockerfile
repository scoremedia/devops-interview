FROM elixir:1.12

RUN apt-get update && \
    apt-get install -y postgresql-client && \
    apt-get install -y inotify-tools && \
    apt-get install -y nodejs && \
    curl -L https://npmjs.org/install.sh | sh && \
    mix local.hex --force && \
    mix local.rebar --force

ENV APP_HOME /app
RUN mkdir $APP_HOME
WORKDIR $APP_HOME

COPY . /app
RUN cd /app && \
    mix deps.get && \
    cd /app/assets && \
    npm install && node node_modules/webpack/bin/webpack.js --mode development

RUN mix deps.compile

CMD ["mix", "phx.server"]