---
title: 'Inhabilitar los {% ifversion projects-v2 %}proyectos{% else %}tableros de proyecto{% endif %} en tu organización'
intro: 'Los propietarios de organización pueden apagar los tableros de proyecto {% ifversion projects-v2 %}de toda la organización {% data variables.projects.projects_v2 %}, {% data variables.projects.projects_v1_boards %} de toda la organización y {% data variables.projects.projects_v1_boards %} a nivel de repositorio{% else %} de toda la organización y de repositorio{% endif %} en una organización.'
redirect_from:
  - /github/managing-your-work-on-github/managing-project-boards/disabling-project-boards-in-your-organization
  - /articles/disabling-project-boards-in-your-organization
  - /github/managing-your-work-on-github/disabling-project-boards-in-your-organization
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Pull requests
shortTitle: Inhabilitar proyectos
allowTitleToDifferFromFilename: true
---

Una vez que inhabilites tableros de proyecto que se usan en toda la organización, ya no se podrán crear nuevos tableros de proyecto a nivel de la organización, y ya no se podrá acceder a ningún tablero de proyecto existente a nivel de la organización en su URL anterior. Los tableros de proyecto en los repositorios de la organización no se ven afectados. {% ifversion projects-v2 %}Estos ajustes aplican a {% data variables.projects.projects_v2 %} y {% data variables.projects.projects_v1_boards %}.{% endif %}

Una vez que inhabilites tableros de proyecto de repositorios en una organización, ya no se podrán crear nuevos tableros de proyecto en ningún repositorio de la organización, y ya no se podrá acceder a ningún tablero de proyecto de los repositorios existentes en la organización en sus URL anteriores. Los tableros de proyecto a nivel de la organización no se ven afectados.


Cuando inhabilitas los tableros de proyecto, ya no ves la información de los tableros de proyecto de manera cronológica o de acuerdo con los [registros de auditoría](/organizations/keeping-your-organization-secure/reviewing-the-audit-log-for-your-organization).


{% data reusables.profile.access_org %}
{% data reusables.profile.org_settings %}
{% ifversion fpt or ghec or ghes > 3.4 or ghae-issue-5658 %}
1. En la sección de "Planeación de código y automatización" de la barra lateral, haz clic en **{% octicon "table" aria-label="The table icon" %} Proyectos**.
{% endif %}
1. Decide si deseas inhabilitar los tableros de proyecto que se usan en toda la organización, los tableros de proyecto de los repositorios de la organización, o ambos. Luego, en "Proyectos":
    - Para inhabilitar los tableros de proyecto que se usan en toda la organización, quita la marca de selección de **Habilitar proyectos para la organización**.
    - Para inhabilitar los tableros de proyecto de los repositorios en la organización, quita la marca de selección de **Habilitar proyectos para todos los repositorios**. ![Casillas de verificación para inhabilitar proyectos para una organización o para todos los repositorios de una organización](/assets/images/help/projects/disable-org-projects-checkbox.png)
1. Haz clic en **Save ** (guardar).

{% data reusables.organizations.disable_project_board_results %}

## Leer más

{% ifversion projects-v2 %}- "[Acerca de {% data variables.product.prodname_projects_v2 %}](/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects)"{% endif %}
- "[Acerca de {% data variables.product.prodname_projects_v1 %}](/articles/about-project-boards)"
- "[Cerrar un {% data variables.projects.projects_v1_board %}](/articles/closing-a-project-board)"
- "[Borrar un {% data variables.projects.projects_v1_board %}](/articles/deleting-a-project-board)"
- "[Inhabilitar los {% data variables.projects.projects_v1_boards %} en un repositorio](/articles/disabling-project-boards-in-a-repository)"
