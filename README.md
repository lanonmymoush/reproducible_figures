# Reproducible_Figures
**Question 3 of Reproducible Figures Assignment**

*Hi reader, 
This repository contains both the R Markdown (.rmd) file and PDF versions of my pipeline (.pdf). 
Enjoy.*

**Question 3C - Partner Feedback**  
**What elements of your partner's code helped you to understand their data pipeline?**  
My partners analysis provided great insight into the background behind the investigated variables, bill length and bill depth. This insight was then further enhanced through the use of code. The comments and notes written besides hashtags in the R code helped me to understand the steps taken to ensure that the code ran and generated the necessary figures. The use of multiple generated functions also made it easier to understand the purpose of the code when a comment was not provided to explain the justification of calling the function. The names of these functions also ensured that the code was both human and computer readable. 

**Did it run? Did you need to fix anything?**  
To get the pipeline to run, I needed to download the corresponding files from their GitHub repository. This was successful however, when attempting to run the code, I ran into some issues in line 51, which attempted to source and call the cleaning and plotting functions. This needed to be altered as a result of the location of the file and working directory. Additionally, the source code attempted to open a file saved as .r as opposed to .R, as suggested in the code, meaning that this also had to be changed. Once these changes were made, it was very easy to run the code. 

**What suggestions would you make for improving their code to make it more understandable or reproducible, and why?**  
I don't believe there are any major suggestions that can be made to improve my partners code, however to make loading the functions more easy, I believe it would be beneficial to save both the plotting and cleaning functions in the same file, perhaps a functions file as opposed to a folder. This would allow the functions to be called more easily as as they are located in the same place regardless of teh location which they are saved on different devices. 
Additionally, to improve general reproduciblity of the code/analysis, I beleive that my partner could have used a Tukey HD test to determine which species are significant different from each other, rather than completing three separate linear regressions. This would be more efficient and would also show how significant the difference is between each group, allowing for inferences to be made about the evolutionary and ecological similarities between species, e.g. overlapping food sources influencing bill depth and length. 

**If you needed to alter your partner's figure using their code, do you think that would be easy or difficult, and why?**  
I believe that altering my partner's figure would be relatively easy. If I wanted to change the scale of the images of the figures depending on the format needed, i.e. if the figure was needed for a poster, presentation, handout, this could be done by altering the scale or resolution of the image, seen in the R chunks which save the figures as a .png and .svg. If saved as an .svg, the image has an "infinite resolution" and can be zoomed in/expanded without becoming pixelated, making the image easier to visualise. 
If I wanted to change the features of the figure, I would have to alter their plotting.R file in which different functions were defined to create the figures. In this code, I could alter the points on the figure, the themes, the axes labels, and also the raw data and change the output of the function accordingly. 

