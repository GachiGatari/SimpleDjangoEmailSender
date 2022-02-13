# SimpleDjangoEmailSender
Simple Django Email Sender Lol that's all that this app done ^-^ 

To start work clone this rep,register at sone free mail sender service(for example SendGrid which i use) and add some fields in EmailDjango/settings.py

```
SECRET_KEY = generate one  
DEFAULT_FROM_EMAIL = 'email from you gonna send message'
RECIPIENTS_EMAIL = ['list of recipients mails']
EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
EMAIL_HOST = 'smtp.sendgrid.net' #add your services
EMAIL_HOST_USER = 'apikey'
EMAIL_HOST_PASSWORD = 'services api key'
EMAIL_PORT = 587
EMAIL_USE_TLS = True
```

For generating django secret key you can use this built-in method
```
from django.core.management.utils import get_random_secret_key  
get_random_secret_key()
```
