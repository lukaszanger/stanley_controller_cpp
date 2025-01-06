# stanley_controller_cpp
Stanley control in C++

![Demo GIF](images/car_stanley.gif)

## Docker Image
### Build
```bash
docker build -t stanley_controller_cpp docker/
```
### Start Docker Container
Check out the CLI tool "docker-run": https://github.com/ika-rwth-aachen/docker-run
```bash
# stanley_controller_cpp
docker-run --mwd stanley_controller_cpp:latest
```

## Run
```bash
# Compile
g++ -I/usr/include/eigen3 -I/usr/include/python3.10 BicycleModel.cpp StanleyController.cpp Animation.cpp Linear_Interpolation.cpp CubicSpline1D.cpp -o stanley_animation -lpython3.10
# Run
./stanley_animation
```



http://www.gnuplot.info/