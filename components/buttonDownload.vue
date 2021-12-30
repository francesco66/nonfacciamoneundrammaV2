<template>
  <div class="dropdown">
    <a class="link grow br3 ba bw1 pa2 bg-animate hover-bg-light-purple bg-black-60 white dib" v-on:click="myFunction()">
      <svg class="bg-white-90" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/></svg>
    </a>
    <div id="myDropdown" class="dropdown-content">
      <a :article="article" v-on:click="onDownloadAsText()">Scarica Txt</a>
      <a v-on:click="onDownloadAsPDF()">Scarica Pdf</a>
    </div>
  </div> 
</template>

<script>
import { saveAs } from "file-saver";

var pdfMake = require('pdfmake/build/pdfmake.js');
var pdfFonts = require('pdfmake/build/vfs_fonts.js');
pdfMake.vfs = pdfFonts.pdfMake.vfs;

pdfMake.fonts = {
  Helvetica: {
    normal: 'Helvetica.ttf',
    bold: 'Helvetica-Bold.ttf'
  },
}

export default {

  props: {
    article: Object
  },

  methods: {
    myFunction() {
      document.getElementById("myDropdown").classList.toggle("show");
    },

    onDownloadAsText() {
      document.getElementById("myDropdown").classList.toggle("show");
      var blob = new Blob(["\n" + this.article.autore + "\n\n" + this.article.titolo + "\n\n" + this.article.text], {type: "text/plain;charset=utf-8"});
      saveAs(blob, this.article.path + ".txt");
      //window.print()
    },

    onDownloadAsPDF() {
      document.getElementById("myDropdown").classList.toggle("show");

      const titolo = this.article.titolo;
      const autore = this.article.autore;
      const testo = this.article.text;

      var docDefinition = {
        content: [
          { text: autore, font: 'Helvetica', fontSize: 16, margin: [ 20, 20 ] },
          { text: titolo, font: 'Helvetica', fontSize: 28, bold: true, margin: [ 20, 30 ]  },
          { text: testo, font: 'Helvetica', fontSize: 14, alignment: 'justify', margin: [ 20, 40 ], lineHeight: 1.5 }
        ],
        pageBreakBefore: function(currentNode, followingNodesOnPage, nodesOnNextPage, previousNodesOnPage) {
          return currentNode.headlineLevel === 1 && followingNodesOnPage.length === 0;
        },
        footer: function (currentPage, pageCount) {
          return { text: "Pagina " + currentPage.toString() + ' di ' + pageCount, alignment: 'right', style: 'normalText', font: 'Helvetica', margin: [ 0, 0, 20, 20 ] }
        },
      };
      
      pdfMake.createPdf(docDefinition).download(this.article.slug + '.pdf');

    }
  }

}
</script>

<style scoped>
/* Dropdown Content (Hidden by Default) */
.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f1f1f1;
  min-width: 120px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

/* Links inside the dropdown */
.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

/* Change color of dropdown links on hover */
.dropdown-content a:hover {background-color: #ddd}

/* Show the dropdown menu (use JS to add this class to the .dropdown-content container when the user clicks on the dropdown button) */
.show {display:block;}

</style>