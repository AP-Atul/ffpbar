# FFmpeg-Progress
Progress bar for FFmpeg using tqdm

## How does it do it?
1. FFmpeg display Duration ```hh:mm:ss.f``` at the start
2. And while encoding it displays Time ```hh:mm:ss.f```
3. Using these values we can count the percentage for the Progress.


## Usage

```python
import ffpbar

bar = ffpbar.Progress()
bar.display(log=str("ffmpeg log"))

# to display the logs, for debugging
bar.display(log=str(""), display_log=True)

# to get the progress (property)
prg = bar.progress
```
