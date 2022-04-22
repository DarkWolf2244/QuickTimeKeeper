# QuickTimer

QuickTimer is a small Python library for timing how long functions take to run.

## Usage

Simply import QuickTimer and call the `time_function` method to time any function you pass in as the parameter. It returns how long the function took to run. Optionally, you can pass in extra args to `time_function` which will be passed into the function to time.

```python
import quicktimer

def fibonacci(n):
    if n < 2:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)

time_taken = quicktimer.time_function(fibonacci, n=10)
print(f"It took {time_taken} ms to run fibonacci(10)")
```
