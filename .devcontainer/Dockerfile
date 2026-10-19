FROM archlinux:latest

RUN pacman -Syu --noconfirm \
    && pacman -S --needed --noconfirm go git shadow zsh \
    && usermod --shell /usr/bin/zsh root \
    && pacman -Scc --noconfirm