# 01 — Linux Server Hardening

Настройка безопасного Ubuntu Server с нуля.

## Что сделано

- SSH: вход только по ключу, пароль отключён, root закрыт
- Пользователи: разграничены роли (admin, developer, monitor)
- UFW: открыты только порты 22, 80, 443
- Fail2ban: бан после 5 неудачных попыток за 10 минут

## Стек

- Ubuntu Server 24.04 LTS
- OpenSSH
- UFW
- Fail2ban

## Конфиги

- `configs/sshd_config` — настройки SSH сервера
- `configs/jail.local` — настройки Fail2ban
