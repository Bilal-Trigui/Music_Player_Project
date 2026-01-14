#Importing base image
FROM nailyudha/tauri:latest

WORKDIR /~/Documents/music_player_project

COPY ./package.json ./cargo.lock ./
RUN cargo i --frozen-lockfile

COPY . .

RUN cargo tauri build