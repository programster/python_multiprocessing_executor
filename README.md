python_multiprocessing_executor
===============================

Python script that takes a path to a file as an argument, and executes each line in that file with a thread a pool equal in size to the cpu_count of the computer, thus fully utilizing the CPU.

## Example Usage
Example file (`/path/to/commands.txt`):
```
ffmpeg -i "01.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/01.flv"
ffmpeg -i "02.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/02.flv"
ffmpeg -i "03.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/03.flv"
ffmpeg -i "04.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/04.flv"
ffmpeg -i "05.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/05.flv"
ffmpeg -i "06.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/06.flv"
ffmpeg -i "07.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/07.flv"
ffmpeg -i "08.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/08.flv"
ffmpeg -i "09.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/09.flv"
ffmpeg -i "10.mkv" -c:v libx264 -ar 44100 -y  -threads 1 "flv/10.flv"
```

Command to call

```
python /path/to/script/main.py /path/to/commands.txt
```
