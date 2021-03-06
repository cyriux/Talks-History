# Modelling Music for DDD practitioners

Most introductory material on music focuses on melody, rhythm and harmony, in the tradition of written classical music. Yet, there's much more than that in music! Playing and creating instruments, sound synthesis, psycho-acoustic perception and illusions, how all this is shaping musical genres, interactions of musicians or DJ with the audience, MIDI production techniques... these all sound like Bounded Contexts to the DDD practitioner. 
Through this session we'll model parts of the rich domain of music with Java and Arduino, in what's really an application of DDD. With some home-made cheesy video, you'll discover and understand music in a new light, and you'll feel like doing your own experiments back at home! 

(fr)
Mieux comprendre Domain-Driven Design en modélisant la musique
Modéliser la musique pour les praticiens de Domain-Driven Design

Quand on pense à la théorie de la musique on pense immédiatement à la mélodie, au rythme et à l'harmonie, dans la tradition de la musique occidentale écrite. Mais ce sujet a tellement d'autres facettes à explorer ! Jouer et inventer des instruments, faire de la synthèse sonore, la perception du rythme, les instruments électroniques et comment tout cela façonne de nouveaux genres musicaux... tout cela sonne comme autant de "bounded contexts" pour les praticiens DDD.

Au travers de cette session nous explorerons des modélisation du domaine riche qu'est la musique avec des fragments de Java ou d'Arduino, dans ce qui constitue de fait une application des notions de DDD. Avec quelques vidéo faites maison un peu kitch, vous découvrirez et comprendrez à la fois la musique et DDD sous un nouveau jour, et vous serez tentés de faire votre propres expérimentations de retour chez vous !


## Additional Information & outline
This talk builds on my past experience building personal research projects I've done around music in Java and Arduino in the past years:

- Creating a *playable* instrument: balancing spontaneity and expressiveness vs difficulty to play in rhythm and in tune (a DIY Light Air Guitar playing a quantized pentatonic scale with a Smart Pitch Bending)
- Literally modelling the internal hardware machine representation (the iconic Hip-Hop Akai MPC) in desktop software (my popular MPC Maid editor for the Akai MPC 500-1000-2000)
- Putting the Groove into equations (Swing %), and how it defined music genres (when introduced in TR808 and Akai MPC), with a concrete Arduino application to groove any MIDI clock, e.g. an Arpeggiator
- Rhythmic Onsets detection & MIDI Sequencing (the auto-slicing tool built-in MPC Maid, showing very simply how it enables basic time-stretching)
- Automatic classification of sound samples by FFT &  Features Extraction with Support Vector Machine (failed experiment but still interesting) 
- Exploring Aesthetics of music: The Wundt Curve and self-similarity of musical patterns, e.g. Fugue, or Rhythmic Layering (a simple Generative Sequencer built with Arduino)
- Shyness and social inhibition, and how anonymity changes everything (we used to make some social experiments of Jam Sessions at home with very shy  non-musicians colleagues, showing how sound effects that make your voice unrecognisable help, plus my past DJ experience dealing with small or large crowds)

I'll show code along with audio and video recordings, e.g. (audio and video recordings)[https://vimeo.com/user1310376] to illustrate the content. The challenge is to keep the talk short and affordable for full beginners, while still showing enough in-depth DDD for the DDD Police :)

(fr)
Ce talk a été présenté une fois (en anglais, non filmée) à NewCraft Bordeaux en octobre 2019, avec de bons retours.

Le thème pourrait aussi être en Mind-the-Geek.

Le format est éducatif et divertissant à la fois, avec une succession de projets musicaux (entrecoupés de mini vidéos) qui servent de support concrets pour présenter des notions abstraites de DDD (domain modeling, bounded context, repository, ubiquitous language, supporting sub-domain, established formalism...) :

- Création d'un instrument de musique jouable avec un équilibre en spontanéité et expressivité (sorte de air guitar sur une gamme pentatonique quantisée et avec possibilité de glissando, en Arduino)
- Modélisation litérale du hardware de la machine icone Hip-Hop Akai MPC, pour en faire un éditeur de programmes en Java
- Détection des battements rythmiques d'une boucle audio MIDI Sequencing (outil d'auto-slicing de boucles, Java)
- Synthèse sonore d'un Wobble façon dubset, avec le synthétiseur modulaire de la librairie open-source Java JSyn

Les liens correspondants pour creuser le sujet sont rassemblés ici : https://gist.github.com/cyriux/55deeeece50a303f6fe87de07c18fbae

## Keywords
music, DDD, modelling, rhythm, groove, how things work, Bounded Contexts, fun, audio, geek
