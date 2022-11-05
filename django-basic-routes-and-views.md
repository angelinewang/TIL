Inside the `base` App:
`urls.py`
```
from django.contrib import admin
from django.urls import path, include

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', include('blogs.urls'))
]
```
= Set up 1. Route for Admin Panel 2. Link to Routes in Other Apps

Ensure other Apps are added to `settings.py` under:
```
INSTALLED_APPS = []

```
