# Simple Monitoring

Минимальная сборка Prometheus, Node Exporter и Grafana через Docker Compose.

Запуск через Docker Compose
1. В корне проекта запустите:
   ```
   docker compose up
   ```
2. Откройте в браузере:
   - Prometheus: http://localhost:9090
   - Grafana: http://localhost:3000

Запуск через Ansible
1. Установите зависимости:
   ```
   ansible-galaxy collection install community.docker
   ```
2. Запустите playbook:
   ```
   sudo ansible-playbook playbook.yaml
   ```

---

To-do
- Защита Grafana (пароль, TLS)
- Добавить пример правил alerting для Prometheus
- Добавить тесты
- Присобачить Github Actions