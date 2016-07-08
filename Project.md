# Final Project

## Description

The final project will consist of a multipart figure that tells a story (often referred to as an 'infographic').  The figure will be uploaded to UBlearns as a PDF file with the underlying R source code.  The topic can be related to the student’s research interests or a separate topic.  

Requirements

1. The graphic(s) must include data from at least two sources that were integrated/merged using R.
2. The underlying data must be publically accessible via the web and downloaded within the R/Rmd script.  If you want to use your own data, you must make it available on a website (e.g. [Figshare](figshare.org)) so that others are able to re-run your code.
2. The graphic should convey at least four dimensions of information (e.g.  latitude, longitude, time, and one more)

Complete submissions will include:

1.	Title (<25 words)
2.	Summary (~250 words) 
3.	Extended caption (~ 1 page)
    * Introduction with description of the question/problem
    *	Methods description
    * Data description
    * Interpretation and discussion of figure(s)
    * Any references

## Formatting

The final project should be organized as a [RMarkdown document](http://rmarkdown.rstudio.com) that includes all the steps necessary to run the analysis and produce the output (figures, tables,etc.).  For examples of similar documents, explore the [RPubs website](https://rpubs.com).    

### Showing Code 
In the output document you can show most of the code except for  particularly long functions or data processing steps (e.g. more than 20 lines or so).   

If some steps of your analysis are time consuming to run (e.g. take more than a few minutes), you might want to pull out those components into a `.R` file to be executed separately.  For example, if your project includes extensive pre-processing, you might have a script (perhaps named `setup.R`)  that performs all the data cleaning and formatting and then saves intermediate files to disk so they can be used in the analysis.  Alternatively, if you want to hide code, you can  use `echo=F` in the code chunk header as explained [here](http://rmarkdown.rstudio.com/authoring_rcodechunks.html)) and then include narrative explaining the processing steps taken in the hidden code.  

### Showing R output
While you should include the code, you should  _not_ include long sections of output from R.  For example, do not include the structure of a raster (e.g. `str(raster)`)  or simple summary of a regression (e.g. `summary(lm)`) in the output document.  To show  results, you can either summarize it into a table (see below) or work it into the text using the inline r code (e.g.,  `'r mean(x)'`).   Remember, you want it to look like a typical scientific manuscript with embedded code.  

### Tables
Please format tabular output (e.g.  summaries of regression models) into markdown tables.  There are several ways to do this, including `kable` function in the 'knitr' package as explained [here](http://rmarkdown.rstudio.com/authoring_rcodechunks.html) and the `xtable` package.  

### Figures
Figures (maps and other graphics) are a vital component of scientific communication and you should carefully plan your figures to convey the results of your analysis.  

### Source and Output Files

You will upload the both the source (`.Rmd`) 	file and a PDF version (not HTML!) of the formatted document.  The PDF version will be graded, the `.Rmd` file will be used only if there are technical questions about the analysis.   You can create the PDF version in either of the following ways:

* Compile the `.Rmd` document to HTML (as we've done in class and explained [here](http://rmarkdown.rstudio.com/html_document_format.html)) and then open the html file in a browser (chrome, explorer, safari, etc.) and print it / save it as a pdf.
* Compile the `.Rmd` document directly to PDF as explained [here](http://rmarkdown.rstudio.com/pdf_document_format.html) 

### References
You should cite any relevant materials (including data sources and methods) in the text using a standard author-date citation format (e.g. Wilson, 2015) and then described in a References section at the end.  You can either compile the references manually (e.g. cutting and pasting the citation into the references section) or use the automated system in RMarkdown explained [here](http://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html).   Other citation styles are acceptable as long as they are consistent, complete, and easy to understand.  

## Grading

To achieve a perfect score a final project would have the following characteristics: 

* **Organization:** The 'story' is very well organized and easy to understand when 'skimming' the document. Clear headings demarcate separate sections. Excellent flow from one section to the next. An abstract or summary at the start of the paper briefly summarises approach and findings. Conclusions at the end present further questions and ways to investigate more. Tables and graphics carefully tuned and placed for desired purpose.
* **Curiosity:** Intense exploration and evidence of many trials and failures. The author looked at the data in many different ways before coming to the final result. The author has gone beyond what was asked: additional techniques from other sources used to help understand/explain findings. The explanation and presentation is creative.
* **Skepticism:** The author suggests multiple explanations for a given finding, and uses multiple tools to explore surprising results. One or two results are presented as the most plausible, but the paper allows for the possibility that results are wrong. The paper is self-critical: What was done well? What was done poorly? What may have been missed? How could it be done better next time? 
* **Grammar:**  All language is well constructed with varied structure and length. The author makes no errors in grammar, mechanics, and/or spelling.
* **Formatting:** Demonstrates mastery of RMarkdown formatting and functions. Paper uses an excellent mixture of headings, tables, and figures.

See the project rubric (see link near top of project submission page) for more details and examples.  

## Project Phases

### Project proposal

The project proposal will be 1 page or less and outline the following:

1.  Introduction to problem/question
2.  Links to inspiring examples:  Include links to a few (~3-5) example graphics found on the internet that are somehow similar to what you want to do.
2.  Proposed data sources
3.  Proposed methods
4.  Expected results

### First Draft

The more complete the first draft, the more feedback I'll be able to provide to ensure an excellent final project.  So it's in your interest to finish as much as possible.  However, the grading of the first draft will be limited to the introduction and methods/data sections.  You should have acquired (downloaded, etc) all the data you plan to use and worked out most of the details of the methods, though you may not have any results or summary figures yet.  I would like to see at least one figure illustrating the data you are working with.  If you include drafts of the results and discussion/conclusion I will also give you feedback on those sections.  

The first draft will be graded using the same criteria as the full project (see above), but I do not expect to see final versions of the discussion and conclusion.  If you have questions or comments, feel free to include them in the draft (e.g., "I'm planning to do X, but I'm not sure how to organize the data appropriately") or as a _comment_ in the UBLearns submission webpage.  

### Final Draft

The final draft will be uploaded to UBLearns at the end of the semester.

**Remember to upload _both_ the .Rmd and the PDF versions! **