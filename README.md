import sys
from time import sleep
import time

def print_line(line, char_delay):
    for char in line:
        print(char, end='', flush=True)
        sleep(char_delay)
    print('')  # Move to the next line

def print_lyrics():
    lines = [
        ("you're all that I want this life", 0.15),
        ("I'll imagine we fell in love", 0.08),
        ("I'll nap under moonlight skies with you", 0.08),
        ("I think I'll picture us, you with the waves", 0.07),
        ("The oceans colors on your face", 0.08),
        ("ll leave my heart with your air", 0.08),
        ("So let me fly with you", 0.15),
        ("Will you be forever with me?", 0.15),
    ]

    delays = [3.2, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 3.2]

    for i, (line, char_delay) in enumerate(lines):
        print_line(line, char_delay)
        time.sleep(delays[i])

print_lyrics()
    
