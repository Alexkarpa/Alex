# lab4
1. **Ознайомився з Docker.**
---
2. **Виконав команди:**
   - sudo docker -v > my_work.log
   - sudo docker -h >> my_work.log
   - sudo docker run docker/whalesay cowsay Docker is fun >> my_work.log
---
3. **Ознайомився з документацією**
---
4. **Створив файл з іменем Dockerfile та замінив посилання на власний Git репозиторій**
---
5. **Створив власний репозиторій на Docker Hub**
---
6. **Виконав команди:**
   - sudo docker build -t alexkarpa/site:django .
   - sudo docker images
   - sudo docker push alexkarpa/site:django
---
7. **Веб-сайт працює**
---
8. 
   - **створив Dockerfile.site**
   - **Виконав білд імеджа:**
       -  sudo docker build -f Dockerfile.site -t alexkarpa/site:monitoring .
       - sudo docker images
       - sudo docker push alexkarpa/site:monitoring
   - **Щоб отримати логи виконав команди:**
     - sudo docker run -it --rm -p 8000:8000 alexkarpa/site:django
     - sudo docker run -it --rm --net=host -v $(pwd)/server.log:/app/server.log alexkarpa/site:monitoring
---