FROM node:12.22.2-alpine
RUN adduser --disabled-password eklovya10 \
    && chown -R eklovya10 /home/eklovya10 \
    && cd /home/eklovya10
USER eklovya10
WORKDIR /home/eklovya10
COPY . .
ENV PORT=5001
RUN npm install
CMD ["npm", "start"]