# AgitSenderLinux
Програма для розсилання "агіток" у цей нелегкий для України час.

Вимагає пароль, тому не для усіх :)

Інструкція:
# Для першого запуску:

1) git clone https://github.com/R0YV0VA/AgitSenderLinux.git
2) cd AgitSenderLinux
3) tar -xf AgitEmailSenderLinux.tar.gz
4) cd AgitEmailSenderLinux
5) wget https://packages.microsoft.com/config/debian/11/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
6) sudo dpkg -i packages-microsoft-prod.deb
7) rm packages-microsoft-prod.deb
8) sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-5.0
9) chmod +x ./AgitMailSender_x64
# Для подальших запусків

1) Створюємо текстовий файл з нашими акаунтами(приклад знаходится у файлі host.txt. Може бути декілька акаунтів)
2) Кидаємо txt файл зі списком email-ів(приклад знаходится у файлі email.txt)
3) Створюємо html файл зі своїм матеріалом(приклад знаходится у файлі index.html)
4) Кидаємо фотки та перейменовуємо як 1.jpg, 2.jpg, 3.jpg ... ( так, працює лише з jpeg. D'oh:( )
5) Виконуємо команди для запуска

для запуска з кореня:

cd AgitSenderLinux; \
cd AgitEmailSenderLinux && \
./AgitMailSender_x64

для запуска з теки:

./AgitMailSender_x64

Приємного користування))
