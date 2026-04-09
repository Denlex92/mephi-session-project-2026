## Операционные системы семейства Unix. Сессионный проект

**Студент:** 332951  


## Описание проекта

Настройка рабочей станции Fedora 43 для работы в локальной сети МИФИ: конфигурация сети, установка ПО, управление файловыми системами, настройка безопасности (DAC, SELinux, Capabilities, PAM) и развёртывание веб-сервера nginx.

## Содержание репозитория

| Файл | Раздел | Описание |
|------|--------|----------|
| `project_history.txt` | Все | История выполненных команд |
| `network_check.txt` | 1.2 | Результаты ping (8.8.8.8, 192.168.1.1) |
| `nginx_recent_logs.txt` | 3.2 | Журнал nginx за последние 5 минут |
| `fstab.txt` | 3.1 | Настройка автомонтирования /dev/sdb1 |
| `selinux_status.txt` | 4.2 | Режим SELinux (Enforcing) |
| `file_contexts.txt` | 4.2 | SELinux-контекст /data/mephi-web |
| `tcpdump_capabilities.txt` | 4.2 | POSIX Capabilities для tcpdump |
| `permissions.txt` | 4.1 | Права и владелец /data/mephi-web |
| `users_groups.txt` | 4.1 | Пользователь mephi-admin и группа mephi-devs |
| `index.html` | 5.2 | Персонифицированная web-страница |
| `curl_output.txt` | 5.2 | Результат curl http://192.168.1.100 |
| `mephi-nginx-screenshot.png` | 5.2 | Скриншот работающего nginx |
| `tcpdump-*.rpm` | 2.2 | Скачанный RPM-пакет tcpdump |

## Конфигурация системы

- **Hostname:** `mephi-2026.domain.local`
- **IP:** `192.168.1.100/24`
- **Шлюз:** `192.168.1.1`
- **DNS:** `8.8.8.8`
- **Веб-сервер:** nginx → `/data/mephi-web`
- **Файловая система:** ext4 (LABEL=MEPHI_DATA) → `/data/mephi-web`
- **SELinux:** Enforcing
- **Пользователь:** `mephi-admin` (группа `mephi-devs`)
