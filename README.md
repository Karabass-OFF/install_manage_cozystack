Скрипт развертывает management-хост, для дальнейшей установки Cozystack.
Как работает скрипт: он скачивает helm, yq, kubectl, docker, talosctl, dialog, nmap, make, kubectl-node-shell, 
talm (еще одна удобная Open Source-утилита от разработчиков CozyStack для конфигурирования Talos Linux — своего рода Helm для Talos),
а потом устанавливает их и раскладывает по каталогам. Весь процесс автоматизирован и сопровождается осмысленными диалогами. 
Кроме того, на хосте поднимаются служба времени NTP, служба доменных имен bind9 и создаются правила 
для организации доступа из кластера в интернет через management-хост. 