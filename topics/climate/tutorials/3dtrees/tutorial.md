---
layout: tutorial_hands_on

title: '3Dtrees: Point cloud processing'
zenodo_link: ''
questions:
- What are LAS data ?
- How can I process and visualise point cloud data ? 
objectives:
- Learn to do point cloud processing
- 
time_estimation: 3H
key_points:
- The take-home messages
- They will appear at the end of the tutorial
contributors:
  autorship:
    - kgerb
    - Marie59

---



General introduction about the topic and then an introduction of the
tutorial (the questions and the objectives). It is nice also to have a
scheme to sum up the pipeline used during the tutorial. The idea is to
give to trainees insight into the content of the tutorial and the (theoretical
and technical) key concepts they will learn.

You may want to cite some publications; this can be done by adding citations to the
bibliography file (`tutorial.bib` file next to your `tutorial.md` file). These citations
must be in bibtex format. If you have the DOI for the paper you wish to cite, you can
get the corresponding bibtex entry using [doi2bib.org](https://doi2bib.org).

With the example you will find in the `tutorial.bib` file, you can add a citation to
this article here in your tutorial like this:
{% raw %} `{% cite Batut2018 %}`{% endraw %}.
This will be rendered like this: {% cite Batut2018 %}, and links to a
[bibliography section](#bibliography) which will automatically be created at the end of the
tutorial.

> <agenda-title></agenda-title>
>
> In this tutorial, we will cover:
>
> 1. TOC
> {:toc}
>
{: .agenda}

# Title for your first section

Give some background about what the trainees will be doing in the section.
Remember that many people reading your materials will likely be novices,
so make sure to explain all the relevant concepts.

## Title for a subsection
Section and subsection titles will be displayed in the tutorial index on the left side of
the page, so try to make them informative and concise!

## Get data

> <hands-on-title> Data Upload </hands-on-title>
>
> 1. Create a new history for this tutorial
> 2. Import the files from [Zenodo]({{ page.zenodo_link }}) or from
>    the shared data library (`GTN - Material` -> `{{ page.topic_name }}`
>     -> `{{ page.title }}`):
>
>    ```
>    
>    ```
>    ***TODO***: *Add the files by the ones on Zenodo here (if not added)*
>
>    ***TODO***: *Remove the useless files (if added)*
>
>    {% snippet faqs/galaxy/datasets_import_via_link.md %}
>
>    {% snippet faqs/galaxy/datasets_import_from_data_library.md %}
>
> 3. Rename the datasets
> 4. Check that the datatype
>
>    {% snippet faqs/galaxy/datasets_change_datatype.md datatype="datatypes" %}
>
> 5. Add to each database a tag corresponding to ...
>
>    {% snippet faqs/galaxy/datasets_add_tag.md %}
>
{: .hands_on}

# Title of the section usually corresponding to a big step in the analysis

It comes first a description of the step: some background and some theory.
Some image can be added there to support the theory explanation:

![Alternative text](../../images/image_name "Legend of the image")

The idea is to keep the theory description before quite simple to focus more on the practical part.

***TODO***: *Consider adding a detail box to expand the theory*

> <details-title> More details about the theory </details-title>
>
> But to describe more details, it is possible to use the detail boxes which are expandable
>
{: .details}

A big step can have several subsections or sub steps:


## Sub-step with **3DTrees: LAS/LAZ Standardization**

> <hands-on-title> Task description </hands-on-title>
>
> 1. {% tool [3DTrees: LAS/LAZ Standardization](toolshed.g2.bx.psu.edu/repos/bgruening/3dtrees_standardization/3dtrees_standardization/1.1.0+galaxy0) %} with the following parameters:
>    - *"Mode"*: `Single File Standardization`
>        - {% icon param-collection %} *"Point Cloud File"*: `output` (Input dataset collection)
>
>    ***TODO***: *Check parameter descriptions*
>
>    ***TODO***: *Consider adding a comment or tip box*
>
>    > <comment-title> short description </comment-title>
>    >
>    > A comment about the tool or something else. This box can also be in the main text
>    {: .comment}
>
{: .hands_on}

***TODO***: *Consider adding a question to test the learners understanding of the previous exercise*

> <question-title></question-title>
>
> 1. Question1?
> 2. Question2?
>
> > <solution-title></solution-title>
> >
> > 1. Answer for question1
> > 2. Answer for question2
> >
> {: .solution}
>
{: .question}

## Sub-step with **3DTrees: LAS/LAZ Standardization**

> <hands-on-title> Task description </hands-on-title>
>
> 1. {% tool [3DTrees: LAS/LAZ Standardization](toolshed.g2.bx.psu.edu/repos/bgruening/3dtrees_standardization/3dtrees_standardization/1.1.0+galaxy0) %} with the following parameters:
>    - *"Mode"*: `Collection Validation`
>        - {% icon param-collection %} *"Point Cloud Collection"*: `output` (Input dataset collection)
>
>    ***TODO***: *Check parameter descriptions*
>
>    ***TODO***: *Consider adding a comment or tip box*
>
>    > <comment-title> short description </comment-title>
>    >
>    > A comment about the tool or something else. This box can also be in the main text
>    {: .comment}
>
{: .hands_on}

***TODO***: *Consider adding a question to test the learners understanding of the previous exercise*

> <question-title></question-title>
>
> 1. Question1?
> 2. Question2?
>
> > <solution-title></solution-title>
> >
> > 1. Answer for question1
> > 2. Answer for question2
> >
> {: .solution}
>
{: .question}

## Sub-step with **3DTrees: SmartTile**

> <hands-on-title> Task description </hands-on-title>
>
> 1. {% tool [3DTrees: SmartTile](toolshed.g2.bx.psu.edu/repos/bgruening/3dtrees_smart_tile/3dtrees_smart_tile/2.0.1+galaxy0) %} with the following parameters:
>    - *"Operation"*: `Tile (COPC normalize + tile + subsample)`
>        - {% icon param-file %} *"Input point clouds (LAZ/LAS)"*: `pc_standardized` (output of **3DTrees: LAS/LAZ Standardization** {% icon tool %})
>
>    ***TODO***: *Check parameter descriptions*
>
>    ***TODO***: *Consider adding a comment or tip box*
>
>    > <comment-title> short description </comment-title>
>    >
>    > A comment about the tool or something else. This box can also be in the main text
>    {: .comment}
>
{: .hands_on}

***TODO***: *Consider adding a question to test the learners understanding of the previous exercise*

> <question-title></question-title>
>
> 1. Question1?
> 2. Question2?
>
> > <solution-title></solution-title>
> >
> > 1. Answer for question1
> > 2. Answer for question2
> >
> {: .solution}
>
{: .question}

## Sub-step with **3Dtrees: Overviews**

> <hands-on-title> Task description </hands-on-title>
>
> 1. {% tool [3Dtrees: Overviews](toolshed.g2.bx.psu.edu/repos/bgruening/3dtrees_overviews/3dtrees_overviews/1.2.0+galaxy1) %} with the following parameters:
>    - {% icon param-file %} *"Point Cloud Collection"*: `pc_standardized` (output of **3DTrees: LAS/LAZ Standardization** {% icon tool %})
>
>    ***TODO***: *Check parameter descriptions*
>
>    ***TODO***: *Consider adding a comment or tip box*
>
>    > <comment-title> short description </comment-title>
>    >
>    > A comment about the tool or something else. This box can also be in the main text
>    {: .comment}
>
{: .hands_on}

***TODO***: *Consider adding a question to test the learners understanding of the previous exercise*

> <question-title></question-title>
>
> 1. Question1?
> 2. Question2?
>
> > <solution-title></solution-title>
> >
> > 1. Answer for question1
> > 2. Answer for question2
> >
> {: .solution}
>
{: .question}

## Sub-step with **3Dtrees: SegmentAnyTree**

> <hands-on-title> Task description </hands-on-title>
>
> 1. {% tool [3Dtrees: SegmentAnyTree](toolshed.g2.bx.psu.edu/repos/bgruening/3dtrees_segmentanytree/3dtrees_segmentanytree/1.2.2+galaxy0) %} with the following parameters:
>    - {% icon param-file %} *"Input Dataset"*: `output_subsampled_res2` (output of **3DTrees: SmartTile** {% icon tool %})
>    - *"Predicted instance dimension name"*: `PredInstance`
>    - *"Predicted semantic dimension name"*: `PredSemantic`
>
>    ***TODO***: *Check parameter descriptions*
>
>    ***TODO***: *Consider adding a comment or tip box*
>
>    > <comment-title> short description </comment-title>
>    >
>    > A comment about the tool or something else. This box can also be in the main text
>    {: .comment}
>
{: .hands_on}

***TODO***: *Consider adding a question to test the learners understanding of the previous exercise*

> <question-title></question-title>
>
> 1. Question1?
> 2. Question2?
>
> > <solution-title></solution-title>
> >
> > 1. Answer for question1
> > 2. Answer for question2
> >
> {: .solution}
>
{: .question}

## Sub-step with **3DTrees: SmartTile**

> <hands-on-title> Task description </hands-on-title>
>
> 1. {% tool [3DTrees: SmartTile](toolshed.g2.bx.psu.edu/repos/bgruening/3dtrees_smart_tile/3dtrees_smart_tile/2.0.1+galaxy0) %} with the following parameters:
>    - *"Operation"*: `Filter (remove overlap-only instances)`
>        - {% icon param-file %} *"Segmented tiles (LAZ/LAS)"*: `output` (output of **3Dtrees: SegmentAnyTree** {% icon tool %})
>        - {% icon param-file %} *"Tile layout JSON (tile_bounds_tindex.json)"*: `output_tile_bounds_json` (output of **3DTrees: SmartTile** {% icon tool %})
>        - *"Border zone width"*: `Derive from tile layout JSON (recommended)`
>        - *"Small cluster reassignment"*: `Enabled`
>        - *"After filtering"*: `Also remap filtered dimensions to another collection`
>            - *"Remap target files"*: `Originals and subsampled targets`
>                - {% icon param-file %} *"Original files (LAZ/LAS)"*: `output_original_copc` (output of **3DTrees: SmartTile** {% icon tool %})
>            - *"Also write one merged output (LAZ)"*: `Yes`
>                - *"Enrich merged output with original attributes"*: `Yes`
>
>    ***TODO***: *Check parameter descriptions*
>
>    ***TODO***: *Consider adding a comment or tip box*
>
>    > <comment-title> short description </comment-title>
>    >
>    > A comment about the tool or something else. This box can also be in the main text
>    {: .comment}
>
{: .hands_on}

***TODO***: *Consider adding a question to test the learners understanding of the previous exercise*

> <question-title></question-title>
>
> 1. Question1?
> 2. Question2?
>
> > <solution-title></solution-title>
> >
> > 1. Answer for question1
> > 2. Answer for question2
> >
> {: .solution}
>
{: .question}

## Sub-step with **3Dtrees: Potree Converter**

> <hands-on-title> Task description </hands-on-title>
>
> 1. {% tool [3Dtrees: Potree Converter](toolshed.g2.bx.psu.edu/repos/bgruening/3dtrees_potree/3dtrees_potree/1.0.2+galaxy0) %} with the following parameters:
>    - {% icon param-file %} *"Point Cloud Files"*: `output_merged_with_originals` (output of **3DTrees: SmartTile** {% icon tool %})
>
>    ***TODO***: *Check parameter descriptions*
>
>    ***TODO***: *Consider adding a comment or tip box*
>
>    > <comment-title> short description </comment-title>
>    >
>    > A comment about the tool or something else. This box can also be in the main text
>    {: .comment}
>
{: .hands_on}

***TODO***: *Consider adding a question to test the learners understanding of the previous exercise*

> <question-title></question-title>
>
> 1. Question1?
> 2. Question2?
>
> > <solution-title></solution-title>
> >
> > 1. Answer for question1
> > 2. Answer for question2
> >
> {: .solution}
>
{: .question}


## Re-arrange

To create the template, each step of the workflow had its own subsection.

***TODO***: *Re-arrange the generated subsections into sections or other subsections.
Consider merging some hands-on boxes to have a meaningful flow of the analyses*

# Conclusion

Sum up the tutorial and the key takeaways here. We encourage adding an overview image of the
pipeline used.