#🛠️ CORREÇÃO DE RELAÇÃO DOS MONITORES – GLPI 11

🔎 Causa

Após a atualização para o GLPI 11, a estrutura de relacionamento de periféricos foi alterada. O plugin ainda utilizava os campos antigos items_id e itemtype, causando falha na associação manual de monitores.

✅ Solução

Foi realizado um fork do plugin original e ajustada a lógica de relacionamento dos periféricos para o novo padrão utilizado pelo GLPI 11.

🔧 Ajuste realizado

Substituição dos campos antigos:

items_id
itemtype

pelos novos campos compatíveis com o GLPI 11:

items_id_peripheral
itemtype_peripheral


# Plugin ocsinventoryng for GLPI
![Logo ocsinventoryng](https://raw.githubusercontent.com/pluginsGLPI/ocsinventoryng/master/ocsinventoryng.png "Logo ocsinventoryng")

![Menu ocsinventoryng](https://raw.githubusercontent.com/pluginsGLPI/ocsinventoryng/master/wiki/menu.png "Menu ocsinventoryng")

* English

This plugin allows you to synchronize with GLPI inventory solution OCS Inventory NG (http://www.ocsinventory-ng.org/fr/).

It replace native mode OCS of GLPI (0.84 version) and use the plugin massocsimport functionalities to provide better compatibility and expandability with OCS.

OCSInventory-NG import automation
It's composed of a script (PHP or Shell) to automate import or synchronisation of computers.
A graphical interface displays the list of scripts running or finished and all the datas related ot them.

WIKI : https://github.com/pluginsGLPI/ocsinventoryng/wiki

Archives (releases) : https://forge.glpi-project.org/projects/ocsinventoryng/files

This plugin is on Transifex - Help us to translate : https://www.transifex.com/yllen/GLPI_ocsinventoryng/dashboard/
