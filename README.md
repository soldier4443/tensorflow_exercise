# tensorflow_exercise

시간날때 짬짬히 하는 tensorflow 연습!

### 레퍼런스

- [Tensorflow Tutorial](https://www.tensorflow.org/get_started/)
- [모두의 딥러닝](http://hunkim.github.io/ml/)
- [Google ML Crash Course](https://developers.google.com/machine-learning/crash-course/)

### 환경

[tensorflow docker image](https://hub.docker.com/r/tensorflow/tensorflow/)를 이용해서
Python 2.7.12 + Jupyter 환경을 구축해서 사용하고 있습니다.

```
docker run -idt -p 8888:8888 --name tensorflow_exercise tensorflow/tensorflow
```

도커 컨테이너를 만들고 `localhost:8888`로 접속해서 작업을 한 다음..

```
docker cp tensorflow_exercise:[directory path] [target path]
docker container stop tensorflow_exercise
```

복사를 하고 컨테이너를 중지합니다.
다시 시작할 때는

```
docker container start tensorflow_exercise
```

이렇게 하면 되긴 하는데
매 번 하는게 번거로우니까 스크립트를 만들어봐야겠음.
