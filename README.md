# Install
* download reveal-md
* install it with npm install
  * in case of trouble with puppeteer
  * sudo npm install -g --unsafe-perm=true

# generation scripts
```shell script
cp -R /datas/dev/moodle/moodle_gitworkspaces/pres/esupdaysrc2021/slides//css/css_esup.css /datas/dev/moodle/moodle_gitworkspaces/moodle35/reveal-md//theme
rm -R ~/Téléchargements/presentation_static
cd slides
reveal-md moodle_rocketchat_esupdays2021.md --static ~/Téléchargements/presentation_static  --css ./css/css_esup.css --theme white --template ./template/reveal.html
reveal-md moodle_rocketchat_esupdays2021.md  -css ./css/css_esup.css --theme white --template ./template/reveal.html --print /datas/dev/moodle/moodle_gitworkspaces/pres/esupdaysrc2021/moodle_rocketchat_plugin_esup_2021.pdf
reveal-md moodle_rocketchat_esupdays2021.md  -css ./css/css_esup.css --theme white --template ./template/reveal.html --print /datas/dev/moodle/moodle_gitworkspaces/pres/esupdaysrc2021/moodle_rocketchat_plugin_esup_2021_speakernotes.pdf
cp -R ~/Téléchargements/presentation_static/* /datas/dev/moodle/moodle_gitworkspaces/pres/esupdaysrc2021/static
cd /datas/dev/moodle/moodle_gitworkspaces/pres/esupdaysrc2021/
git add -A
git commit -m 'moodle RC esup days 2021'
git push
```


# spearker view
S
