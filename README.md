# requirements:
```
	Django==3.0.7
	Pillow==7.1.2
```
# Installation:

- Create a django project.
	
	
- Pull this repository into your django project in the same directory where manage.py file is.
	
	
- Add this app into your settings.py file's INSTALLED_APPS section
```
	INSTALLED_APPS = [
    		'django.contrib.admin',
    		'django.contrib.auth',
    		'django.contrib.contenttypes',
    		'django.contrib.sessions',
    		'django.contrib.messages',
    		'django.contrib.staticfiles',
    		'users'
	]
```
	
- All the following code into your project's settings.py file
```
	TEMPLATE_DIR = os.path.join(BASE_DIR, 'templates')
	STATIC_DIR = os.path.join(BASE_DIR, 'static')
	MEDIA_DIR = os.path.join(BASE_DIR, 'media')
	STATICFILES_DIRS = [STATIC_DIR, ]
	MEDIA_ROOT = MEDIA_DIR
	MEDIA_URL = '/media/'


	LOGIN_URL = 'knowme/user_login'

	AUTH_USER_MODEL = 'users.Account'
```
