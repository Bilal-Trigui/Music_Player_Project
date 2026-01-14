#Importing base image
FROM nailyudha/tauri:latest

#setting work directory for app
WORKDIR /~/Documents/music_player_project

#copies and installs dependencies
COPY ./package.json ./cargo.lock ./
RUN cargo i --frozen-lockfile

#copies rest of the files
COPY . .

#runs build command
RUN cargo tauri build