# Speaker_recognition
convergys_internship
This code uses MFCC spectrograms to indentify different speakers based on the mfcc of the voice of the speaker.

The code is divide into 3 parts and a subset of the original dataset (http://www.repository.voxforge1.org/downloads/SpeechCorpus/Trunk/Audio/Main/16kHz_16bit/) 
is used using voice of 3 individuals from this dataset,

To run the code download any 3 individual voices of a person from the fore-mentioned dataset.

Keep all .wav files in different filder names in the format

Speaker1
  a.wav
  b.wav
  ...
Speaker2
  a.wav
  b.wav
 
 and so on
 
 Replace directory name as according to your system in audioMFCC to convert all .wav files to .png(Image files)
 run the move files code to seperate .wav file from .png and move them to a new folder
 
Make folder Train
having .png files of different speakers in differnt folders as shown above
similarly make a valid folder and use some of the images as validation/testing images


Run voice_CNN after moving files to seperate folders as stated above.

As of now we get a train accuracy of 88% and val/test accuracy of 100%(due to small size of validation data)
But there are some aspects that can be further improved in this code
1. Using MFCC features instead of MFCC images though it might result in  a slight better accuracy we can explorre this option.
2. Using/ Modifying the CNN structure
3. Using RNN's as they prove good and work well when the data is based on patterns.

