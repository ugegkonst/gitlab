## Дополнительные материалы для выполнения домашних заданий из блока "Введение в DevOps"


#Домашнее задание по GitLab 8.3 Егор Угнивенко*

##Задание 1

![runner param screen](https://github.com/ugegkonst/gitlab/blob/ca60f9657ea935967302cfcae1b61f65e64a0c7e/img/Screenshot%20from%202023-03-13%2022-12-30.png)


##Задание 2.
```YAML:
stages:
  - test
  - build

test:
  stage: test
  image: golang:1.17
  script: 
   - go test .

build:
  stage: build
  image: docker:latest
  script:
   - docker build .
```

![jobs screen](https://github.com/ugegkonst/gitlab/blob/b0fd57e195868bf54f16c2a5b66a54657d3d8529/img/Screenshot%20from%202023-03-15%2023-54-07.png)
![job 1 in details](https://github.com/ugegkonst/gitlab/blob/b0fd57e195868bf54f16c2a5b66a54657d3d8529/img/Screenshot%20from%202023-03-15%2023-54-13.png)
![job2](https://github.com/ugegkonst/gitlab/blob/b0fd57e195868bf54f16c2a5b66a54657d3d8529/img/Screenshot%20from%202023-03-15%2023-55-18.png)



