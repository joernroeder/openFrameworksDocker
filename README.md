# openFrameworks Docker image
This is an Ubuntu 15.10 docker instance with openFrameworks pre-installed.

Use this for running openFrameworks apps easily on a headless instance, useful for
image processing services for example.

## Usage
The most basic usage is like this:
```
cd [YOUR_OF_APP]
docker run -v $(PWD):/app -t -i halfdanj/openframeworks:0.9.3
```

This will download the openframeworks image, and start it with your current
directory mounted. It will then compile your source code, and run it in release.
