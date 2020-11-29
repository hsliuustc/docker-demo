# demo
docker demo

Build

```
docker build -f Dockerfile -t docker-demo  .
```

Run
```
docker run -ti docker-demo /bin/bash -c "source activate hero && cd src/app && python main.py"
```


To save output in local path, run
```
docker run  -v $(pwd)/data:/root/data -v $(pwd)/src:/src hsliuustc/docker-demo /bin/bash -c "source activate hero && cd src && python main.py"
```


To save output in local path, run
```
docker run  -v $(pwd)/data:/root/data -v $(pwd)/src:/src dockerdemo /bin/bash -c "source activate hero && cd src && python main.py"
```