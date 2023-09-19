# SOUNDING_LAB
Sounding Lab Report

Radiosonde Exercise

Introduction
The aim of this exercise is to analyse data from an atmospheric sounding and compare the
observed vertical profile above Marsta, Sweden to the synoptic weather pattern at the time the
sounding took place. You should hand in a group report including plots and discussion for one
of the events according to the questions below.

Method
You will receive the following files:
• 20130926.txt
• 20140925.txt
• 20210920.txt
• data header.txt
• WXMAP20130926_00UTC
• WXMAP20140925_00UTC
• WXMAP20210920_00UTC

You will be assigned one of the events. On Studium, one can find the weather maps for 26th
September of 2013, 25th September of 2014 and 20th September of 2021 in the files
WXMAP$date$_00UTC. The sounding data for these three dates are found in the .txt files
20130926.txt, 20140925.txt and 20210920.txt with variables organized in columns following
the header described in data header.txt

You can use any analysis software you'd like, you are welcome to be creative in how you handle
the data. With Python you can use Pandas to import the data using the following command:
“data=pd.read_csv("file.txt", delim_whitespace=True , header=None)”. I can suggest to
explore MetPy library to analyse the radio sounding. If you are using MATLAB you can use
"Import Data" tool if you are having problems loading the sounding text files for your analysis
otherwise using the following line should work: “data=load('file.txt');”.

Analysis
Your report should answer the following questions:

1. What is the height of the atmospheric boundary layer?
2. Did the balloon reach the tropopause? If so, at what height is the tropopause located?
What is the pressure and temperature at that elevation?
3. Can you see a front at any height?
4. Are there any layers with clouds?
5. Are there any unstable layers in the profile? Stable layers? Do you see any inversions?
6. What happens to the wind speed as one rises through the column? What is the
difference between the wind speed in and above the boundary layer?
7. Use the Cumulus formula to calculate the cloud base and saturation temperature.
8. Are there any possibilities for deep convection? Find the Level of Free Convection
(LFC), Equilibrium Level (LEQ) and estimate the Convective Available Potential
Energy (CAPE) in the column. (Use the Oredsson or Skew-T Log P diagram)

Finding the boundary layer height
To do this the easiest way, make a subplot of relative humidity (RH), potential temperature,
wind direction and rising speed of the balloon against the altitude up to 2000 m. The height
of the boundary layer is often visible as a sharp inversion in the potential temperature. The
rising speed of the balloon is a good indicator of the turbulence in the air. Typically, the rising
speed is jumpy in the boundary layer and then stabilizes to a smoother ascent once the balloon
reaches more laminar flow above the boundary layer.

Other hints
Plot temperature, wind direction, wind speed, potential temperature, adiabatic equivalent
potential temperature 𝜃𝑎𝑒, and relative humidity up to maximum altitude. Closely take note
of what you see. If there are any frontal passages they can often be identified with a veering
wind profile or by a difference in 𝜃𝑎𝑒, signalling different air masses. Use the weather maps
provided to connect the observed vertical profile to the larger scale weather pattern. Useful
links for past weather:
Meteociel - Cartes du modèle numérique GFS pour l'Europe
Home page wetterzentrale.de (Archive)


Good luck & have fun! Feel free to ask any questions if you are stuck! The final report is
due 8th of October before 23:59.
