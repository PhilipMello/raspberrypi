# How to install Docker on Raspberry

- Install Docker CLI
  ```bash
  curl -sSL https://get.docker.com/ | CHANNEL=stable sh
  ```
    - Enable and start Docker
    ```bash
    sudo systemctl enable --now docker
    ```
    - Add your current user to Docker group
    ```bash
    sudo usermod -aG docker $USER
    ```
