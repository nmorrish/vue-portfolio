# Vue Portfolio
This is my online portfolio done using Vue.js
It's a single page to show my skills and some of my work. 

#See this website live
Website is live at https://m-is.net

#Deploying project
move to the project directory in the CLI and run 'npm run build'

Move all files in the './dist/' directory to the server using ftp. 


#Components
Vue.js could be considered overkill for what I need, however, the ease at which Vue allows a page to be split into compenents helps to speed up development and allows for greater scalability as I add projects to my portfolio. Here are the major components:

#./src/components/ProjectPreviewComponent.vue
-Usage-
Import:
<script setup>
	import ProjectPreviewComponent from './ProjectPreviewComponent.vue'
</script>

Display:
<ProjectPreviewComponent previewTitle="..." previewImage="./assets/img.png" siteUrl="https://..."/>

Displays an image of the project with the project title overlayed. The entire component is an anchor that can link the the full project. 
Takes 3 arguments:
 -previewTitle: the title of the project
 -previewImage: path to the image of the project. In this project, they are stored under './assets/'
 -siteUrl: path to a website displaying the project so people can look at it in full.


#./src/icons/*.vue
Each component in this directory is an svg object that is used for the icon of each skill on the portfolio.

-Usage-
Import:
<script setup>
	import IconName from './icons/IconName.vue'
</script>

Display:
<DotNetLogo/>

#./src/components/ExternalMediaComponent.vue
Displays the links to github, linkedIn, and email. Should the links to any of those change, they can be updated here.
