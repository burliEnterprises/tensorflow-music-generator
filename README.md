# tensorflow-music-generator
<img src="https://github.com/koflerm/tensorflow-music-generator/blob/master/music.png?raw=true"/>
</br>
generates music (midi files) using a Tensorflow RNN

Read more about it on  Medium: https://medium.com/@m_ko/deep-learning-with-tensorflow-part-3-music-and-text-generation-370cf37bb071

Hear a demo of the result here:
https://www.youtube.com/watch?v=5wZIQ9XHNns&feature=youtu.be


## Overview
Use TensorFlow to generate short sequences of music with a [Restricted Boltzmann Machine](http://deeplearning4j.org/restrictedboltzmannmachine.html). 
Original code comes from YouTube, see here: (https://youtu.be/ZE7qWXX05T0)

## Dependencies

  * [Tensorflow](https://www.tensorflow.org/versions/r0.10/get_started/os_setup.html)
  * pandas
  * numpy
  * msgpack-python
  * glob2
  * tqdm 
  * python-midi
  
Use [pip](https://pypi.python.org/pypi/pip) to install any missing dependencies (pip install --upgrade ... ) 

### Dependencies on Windows with python3
```
    pip3 install pandas
    pip3 install msgpack-python
    pip3 install numpy
    pip3 install glob2
    pip3 install tqdm
    pip3 install py-midi
```

## Basic Usage
To train the model and create music, simply clone this directory and run
```
python rbm_chords.py
```

The training data goes in the pop_music_midi folder. You have to use MIDI files. You can find some [here](http://www.midiworld.com/files/).
I have already added pop songs.
Training will take 5-10 minutes on a modern laptop. The output will be a collection of midi files.

## Credits

The credit for this code goes to [dshieble](https://github.com/dshieble) and [llSourcell](https://github.com/llSourcell/Music_Generator_Demo)

Have fun!
