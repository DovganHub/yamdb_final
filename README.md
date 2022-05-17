# api_yamdb
api_yamdb
# Учебный проект infra_sp2
### Описание
Проект служит для размещения проекта api_yamdb в Doker для разворачивания проекта в любых операционных системах.
Созданы три образа
### Технологии
Doker
### Запуск проекта 
- запуск контейнера 
```docker-compose up -d --build
```  
- запуск миграций
``` 
docker-compose exec web python manage.py migrate
```
- создание суперпользователя
```
docker-compose exec web python manage.py createsuperuser 
```
- собрать статику
```
docker-compose exec web python manage.py collectstatic --no-input 
```

### Авторы
Александр


![example workflow](https://github.com/DovganHub/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)


http://51.250.32.175/admin/login/?next=/admin/