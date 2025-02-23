# Project.Sonata




## Ideas and train of thoughts 

to write a music one needs to take several elements into consideration : 
1. first and for most is the time signature . this defines the enigine of the pice. the time signature stays most of the times constant and doesnt change during a piece .
2. Form . Form is often less considered to be important when writing a music piece. However it is one of the most deterministic parts of the music and acts as the Frame of the musical piece. for instance a sonata is a sonata because of its form.
3. chord progression . to move between different harmonic functions is a conversation starter in a music. this is also related to form of the musical piece and cannot be diffrenciated . Non the less writing the chord progression designs the story of the musical piece.
4. another essential part of a musical piece is melody writing. melody writing is the detail work of the musical piece.Melody is what makes a musical pice unique. Although, melodical themes can be infinitly variant, in ocntext of a musical piece , they depend on the time signature, forma and harmonical background in the piece at given time.

writing a musical piece often starts with a unique idea like a melodical theme or an interesting chord progression. However, in order to put these creative inspirations into context of a musical piece, one needs to decide on time signature and form and then continue that train of thought and finish the piece trying not to lose the integrity of the piece and not going very far away from the original melodic motive , but also avoid repeating to keep the whole piece still interesting enough for the listener to follow. 

The main objective of this project is to teach machines to make a complete piece of music. However not just a random piece , since that is of no humans interest. People like to see their own ideas come to the reality and they like to own the credit. The feeling of competeing with a machine is not what this project is aiming to give its users. This project is aimed to be a tool inorder to help musicians, and hobby musicians to write a piece of music based on their own unique inspiring motives and melodies. 

  We aim to start small but make it expandable. 

  The basic idea is that the machine takes an input in form of a melodical motive, or some chord progression, form of the music, time signature and also maybe style of a musician, and continue expanding the given motive in order to compeletly write a musical piece. 

  
  The completed project does the following :

  1.it automatically decides on time signature (can also be given by user) , musical form ( can be infered from the music style and artist) , and creates chord progression based on these given information. 
  2.given a melody, it will generate chord progression, form , and the rest of the meloidcal variation and writes a compelete musical piece 

  to achieve this , the author thinks that the follwoing steps are neccesary:

  we need 3 models :   

  1. Model 1 : has understanding of musical form. this needs to look at the whole musical piece to understand chord patterns, melody patterns and undestand the repetitions that comes with specific form
  2. Model 2 : has understanding of musical chord progression . this model will be given the form as a helpper input, and a chord, and generates chord progressio until the end of the song or musical piece
  3. Model 3 : writes melody based on the chord patterns given to the model .

It is clear for the author that a large enough GPT like model  , such as GPT 3.5 can learn all 4 elements , given enough parameteres and large enough datasets. however, aim is to make the smallest possible model that can achieve our goal.
  

## Prototyping 


  in order to make a prototype we will first aim to solve one of these problems :
  1. chord progression based on given style and musician
  2. melody writing based on given style and musician

### Todo : 


### Done sofar :

1. first model was trained on pretrained GPT2 model and was able to generate 3 notes :)
a. data set : maestro midi dataset converted to midi text , having composer name and piece name 
b. Tokenizer was the extended GPT2 model tokenizer with midi tokens

_________________
Conclusion : 
it is possible to achieve the task using GPT like models . it worked at the end . 
However, tokenizer was too large . we extended 50000 token size with 300 midi tokens . 
sequence size can be optimized in a way . 


