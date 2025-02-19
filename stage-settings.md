---
title: Stage Settings
parent: Stages
has_children: false
nav_order: 2
layout: page
---

# Stage Settings
To find out more about what stages are, [click here.](../stages.html)

## Administrators only 

Administrators can Add a Stage. Read more about how to [add a stage here.](../stages.html)

Once a stage is added, administrators can edit the settings of that stage by selecting the *"Stage name" > Settings* from the side navigation pane.

Under Settings you can enable the stage by switching the 'Enable Stage' button. 
Enabling a stage allows members of the project to begin reviewing in that stage. You can temporarily disable while you configure the stage, and re-enable when ready.

Note that it is not possible to delete a Stage once it has been added to a project. It is only possible to edit the settings of the stage for example you can disable the stage so that it is not available to Reviewers on the project.


![Stage Enable](/figs/Fig_Stage-Settings-Advanced-settings-enable_NEW.png)


## Review Mode

Under "Review Mode", project administrators can configure various settings for stages with screening and annotation, such as: include and decide which capabilities to add to your stage, e.g. screening, annotation and data extraction, by selecting these modes using the checkboxes.  

### Screening
Screening Settings can be edited by clicking the link ‘Click for editing screening settings’. If you choose both screening and annotation, you will be asked to choose how to combine these tasks under "Study Selection Settings". 

Specifically, the options are: 
- All studies require screening, but annotation is optional 
- All studies require annotation, but screening is optional 
- All studies require both screening and annotation


![Stage Options](/figs/Fig_stage_options_NEW.png)


Read more about these options in [Stages.](../stages.html)

### Annotation
If annotation is selected, multiple options are presented. 

__Required Annotators per Study__ - Project administrators can adjust the “required annotators per study” for their project. This represents the number of independent reviewers who can annotate each study. Adjust the number in the input box by using the arrows or simply type a number. This input box only accepts whole numbers. 
We recommend two independent reviewers annotate each study in your systematic review, this is typically required for publication in scientific journals, and this is the default option. For student projects or other projects where two independent reviewers are not required to annotate each study there is an option to decrease the number of reviewers. 


![Required Annotators per Study](/figs/Fig_Stage-Advanced-settings-annotation-settings_NEW.png)


__Limit Incomplete Sessions__ - Project administrators can now limit how many annotation sessions with the status “in progress” each reviewer on their project can have. When a reviewer reaches this limit, they will not be able to begin annotation of further studies without completing annotations on these "in progress" or saved studies. Therefore this number is the maximum number of "in progress" or studies with incomplete annotations a reviewer can have saved.
Adjust the number in the input box by using the arrows or simply type a number. This input box only accepts whole numbers. Currently, by default, this option is ticked and the limit is set to 100 studies. To reduce the number of annotation sessions a reviewer can have in progress at one time, reduce the number.


![Limit Incomplete Sessions](/figs/Fig_Stage-Advanced-settings-maximum-incomplete-sessions_NEW.png)


#### Advanced Annotation Settings

By clicking the arrow to reveal the “Advanced Settings”, there are multiple options presented.


![Advanced Annotation Settings Arrow Button](/figs/Fig_Stage-Settings-Advanced-settings-arrow-button_NEW.png)


__Team-Excluded Studies__ - To configure advanced settings for stages with “annotation”, project administrators can choose to show or hide studies that have been sufficiently screened and excluded by reviewers in the project. 


![Team-Excluded Studies](/figs/Fig_Stage-Advanced-settings-hide-excluded-studies_1_NEW.png)


Hiding studies (ticking the checkbox "Hide Studies") will mean that the annotations are not presented to other reviewers, and if a reviewer has this study in the “incomplete studies” section, it will be removed.
Studies that are team-excluded before a reviewer starts annotation will never be randomly presented to that reviewer. However, they remain accessible via direct links.


![Hide Excluded Studies](/figs/Fig_Stage-Advanced-settings-hide-excluded-studies_2_NEW.png)


There are 2 options for how the statistics for excluded studies are grouped, and each option has further configurable options indicating how the statistics for excluded studies are presented in the annotation progress bar: 

1) When "Hide Studies" is not ticked: 
* Group with Incomplete/Completed
* Separate Sections


![Hide Excluded Studies - grouping 1](/figs/Fig_Stage-Advanced-settings-excluded-grouping-1_NEW.png)


2) When “Hide Studies” is ticked: 
* Separate Sections
* Group with Unavailable

Where "Unavailable" means that the excluded studies are categorised as "Unavailable" on the progress bar.


![Hide Excluded Studies - grouping 2](/figs/Stage-Advanced-settings-excluded-grouping-2.png)

