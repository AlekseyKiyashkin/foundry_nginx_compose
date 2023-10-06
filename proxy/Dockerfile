FROM nginx:1.24-bullseye

COPY ./foundryvtt.kiiashkin.net /etc/nginx/sites-available/
RUN ln -s /etc/nginx/sites-available/foundryvtt.kiiashkin.net /etc/nginx/sites-enabled/

CMD ["nginx", "-g", "daemon off;"]