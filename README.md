PROJECT ARCHITECTURE:::

          GitHub → Jenkins → Ansible → EC2 Server → Application Deployed


FOLDER STRUCTURE:::

            ansible-cicd-project/
          ├── Jenkinsfile
          ├── inventory
          ├── playbooks/
          │   ├── install-deps.yml
          │   ├── deploy.yml
          │   └── start-service.yml
          └── src/
              └── index.html
