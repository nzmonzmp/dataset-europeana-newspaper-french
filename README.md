**Europeana Newspapers French corpus (text format)**

source : http://api.bnf.fr/europeana-newspapers-french-corpus-text-format



This data set contains the text of the newspapers collections processed during the Europeana Newspapers project.

Sommaire

    -
    Dataset Content
    -
    Context
    -
    Formats
    -
    Reuse Examples of this Dataset
    -
    APIs and Datasets in relation with this Dataset

Dataset Content

This dataset contains OCR's transcription of the text of about 2 million pages from Gallica's press collections. The format used is JSON.

All the digitized documents in Gallica of the following newspapers titles are available:

    L’Action française : http://gallica.bnf.fr/ark:/12148/cb326819451/date
    Le Constitutionnel : http://gallica.bnf.fr/ark:/12148/cb32747578p/date
    La Croix : http://gallica.bnf.fr/ark:/12148/cb343631418/date
    L’Echo de Paris : http://gallica.bnf.fr/ark:/12148/cb34429768r/date
    Le Figaro : http://gallica.bnf.fr/ark:/12148/cb34355551z/date
    Le Gaulois : http://gallica.bnf.fr/ark:/12148/cb32779904b/date
    L’Humanité : http://gallica.bnf.fr/ark:/12148/cb327877302/date
    L’Intransigeant : http://gallica.bnf.fr/ark:/12148/cb32793876w/date
    Le Journal des débats politiques et littéraires : http://gallica.bnf.fr/ark:/12148/cb39294634r/date
    Le Matin : http://gallica.bnf.fr/ark:/12148/cb328123058/date
    Ouest Eclair (éditions de Caen, Nantes, Rennes) :
        http://gallica.bnf.fr/ark:/12148/cb41193642z/date
        http://gallica.bnf.fr/ark:/12148/cb41193663x/date
        http://gallica.bnf.fr/ark:/12148/cb32830550k/date
    Le Petit Journal : http://gallica.bnf.fr/ark:/12148/cb32895690j/date
    Le Petit Journal illustré supplément du dimanche : http://gallica.bnf.fr/ark:/12148/cb32836564q/date
    Le Petit Parisien : http://gallica.bnf.fr/ark:/12148/cb34419111x/date
    La Presse : http://gallica.bnf.fr/ark:/12148/cb34448033b/date
    Le Siècle : http://gallica.bnf.fr/ark:/12148/cb32868136g/date
    Le Temps : http://gallica.bnf.fr/ark:/12148/cb34431794k/date
    L’Univers : http://gallica.bnf.fr/ark:/12148/cb34520232c/date

It is organized by newspaper title, year and publication date (one JSON file per issue). Example for the 1884, June 15 issue:

le_petit_journal_illustre_supplement_du_dimanche.zip/1884/18840615/18840615.metadata.fulltext.json

 
Context

This corpus was produced during the European research project "Europeana Newspaper" (2012-2015).

    http://www.europeana-newspapers.eu/

Formats

Each JSON file contains metadata informing of the title, publication date and ARK identifier of the document in Gallica:

{
	"title": [
		"Le Petit Journal illustré Supplément du dimanche"
	],
	"source": [
		"Bibliothèque nationale de France",
		"http://gallica.bnf.fr/ark:/12148/bpt6k7155522",
		"Metadata aggregated by The European Library",
		"Metadata provided by National Library of France "
	],
	"description": [
		"1884/06/15 (Numéro 1)."
	],

Textual content is stored in the contentAsText field.  Paragraph end is encoded with the \n character. Any hyphens at the end of the line have been removed.

Other metadata are also available:

    ARK identifier of the newspaper title record in the BnF catalogue:

"relation": [
"http://data.theeuropeanlibrary.org/Collection/a0599",
"Notice du catalogue : http://catalogue.bnf.fr/ark:/12148/cb32836564q", …

    Document identifier in the European digital library TEL:

"identifier": [ "http://data.theeuropeanlibrary.org/BibliographicResource/3000117762175",
"http://www.theeuropeanlibrary.org/tel4/newspapers/issue/3000117762175",
"http://www.theeuropeanlibrary.org/tel4/newspapers/issue/fullscreen/3000117762175",...]

    Estimated OCR quality rate (in % of correct words) :

"format": [
"[OCR confidence] 0,806267"]

 
Reuse Examples of this Dataset

    https://scoms.hypotheses.org/657
    https://scoms.hypotheses.org/799
    https://numapresse.hypotheses.org/

APIs and Datasets in relation with this Dataset

The "Gallica OCR" API enables OCR files of digital documents to be obtained from their ARK identifier:

http://gallica.bnf.fr/RequestDigitalElement?O=bpt6k5773155v&E=ALTO&Deb=1