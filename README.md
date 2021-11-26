Source: https://gitlab.com/gitlab-org/gitlab/-/issues/23911#note_215199418

1. Aggiunto il mapping dell'ip nell'etc/hosts -> sudo nano /etc/hosts 
    127.0.0.1 gitlab-web
2. Setuppare il runner (one time job): docker-compose run gitlab-runner-register
3. Quando ha terminato lanciare gitlab+runner con comando: docker-compose up gitlab-web gitlab-runner
4. Dal browser raggiungere gitlab all'indirizzo: gitlab-web:8080. Accedere con utente: root - Test123#