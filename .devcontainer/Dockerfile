FROM archlinux:latest

RUN pacman -Syu --noconfirm \
    && pacman -S --needed --noconfirm base-devel go git shadow sudo zsh \
    && useradd --create-home --uid 1000 --user-group --shell /usr/bin/zsh vscode \
    && printf 'vscode ALL=(ALL) NOPASSWD: ALL\n' > /etc/sudoers.d/vscode \
    && chmod 0440 /etc/sudoers.d/vscode \
    && pacman -Scc --noconfirm

USER vscode