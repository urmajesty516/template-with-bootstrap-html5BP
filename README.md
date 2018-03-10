# Template with bootstrap and html5BP
Teach you how to create a template with bootstrap and html5 boilerplate
<h2>Description</h2>
<p>Setting up a project with html5 boilerplate and bootstrap can save loading proccess and also, be easy for later maintenance.</p>
<h2>Install</h2>
<p><strong>Download:</strong><br/>
HTML5 boilerplate open source code from the link: <a>https://html5boilerplate.com/</a><br/>
Bootstrap open source code from the link: <a>https://getbootstrap.com/docs/3.3/ (<strong>v3.3.7</strong>)</a><br/>
A LESS compiler: I'm using WinLess which is a free open source tool: <a>http://winless.org/</a><br/>
fontawesome icons: <a>https://fontawesome.com/</a><br/>
</p>
<h2>Configuration</h2>
<p>
  <ol>
    <li>Open up bootstrap folder>less folder>bootstrap.less>compile>set output path: project folder/css>get bootstrap.css</li>
    <li>Open up bootstrap folder>less folder>copy all> project folder/less/>create a folder called bootstrap> paste all</li>
    <li>If using glyphicon, open up bootstrap folder>less folder>copy all> project folder/less> create a new folder called bootstrap>paste all</li>
    <li>If using fontawesome, under fontawesome directory, copy files in the less folder in web-fonts-with-css, create a new folder called fontawesome and paste all into it.</li>
    <li>Open up bootstrap folder>less folder>bootstrap.less>copy> project folder/less/bootstrap/> create __main.less>paste all> add <pre>@import "font-awesome/fontawesome.less";</pre></li>  
    <li>open up WinLess, compile __main.less to project/css/</li>
    <li>Open up project folder (HTML5 boilplate), delete doc folder, create fonts/webfonts (depends on you are using glyphicon or fontawesome) folder under main directory</li>
    <li>Open up fontawesome folder> webfonts>copy files under project folder/webfonts</li>
    <li>Or, open up bootstrap folder/fonts> fonts>copy files under project folder/fonts</li>
    <li>Open up bootstrap folder>js>copy all>project folder/js>create a new folder called bootstrap/paste all.</li>
    <li>If using fontawesome, go to fontawesome/web-fonts-with-css/css/fontawesome-all.min > copy and paste > project folder/css. If using glyphicon, do nothing.</li>
    <li>Delete the main.css under project/css because you will compile your own one later.</li>
    <li>Edit plugin.js in project folder>bootstrap folder/dist/js/bootstrap.js>copy>paste under the jquery comment of plugin.js</li>
    <li>Place a .htaccess file in webfonts/fonts folder with content:<br/>
      <p>
        <img src="https://i.imgur.com/L0E2LoG.png" width="300">      
      </p>
   </li>
  </ol>
</p>

<h2>Directory Structure</h2>
<pre>
project/
      css->YOUR_main.css | bootstrap.css | fontawesome-all.min.css
      img
      js-> boostrap/
        -> vendor/
        -> main.js | plugins.js
    less-> boostrap/
        -> font-awesome/
        -> __main.less 
webfonts-> .htaccess | all the files from fontawesome with suffix file names such as .eot, .woff, ect.     
</pre>

<h2>Usage</h2>
<p>Now you are ready to go! Customize your less file under project/less, and add @import to your __main.less, at last, compile to your main.css</p>
