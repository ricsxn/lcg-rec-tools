lcg-rec-tools
=============

LFC file catalog tools for recursive lcg-* commands

LCG based file catalog and related storage elemement interactions have been kept separated 
by the current gLite/LCG2.0 middleware. 
Specialized CLI tools exist in order to handle with the LFC catalog or with the storage elements. 
Tools interacting with the file catalogs have a prefix: 'lfc-*' while commands interacting with the
storage elements have a prefix: 'lcg-*'. 

Although the use of these commands is really easy and flexible, all of them do not allow to operate 
recursively into a catalog directory. Operations like copy an entire directory content from a file catalog
to a local path in the UI(or Worker node) or viceversa with a single command are not possible using the 
current lcg-*/lfc-* commands. 

A new set of tools have been written in order to allow recursive operations over a directory, involving 
copy from file catalogs to local filesystem and viceversa in a single operaton. 
Other similar tools have been developed in order to cancel a whole catalog directory tree anr removing related 
files from the storage elements as well (all replicas), or add new replicas etc.

All these tools accept several options as parameters allowing the user to configure the commands accordignly 
to their needs. Since the use of these commands make use of lcg-*/lfc-* CLI tools, a valid proxy
with voms extentions is needed exactly like in other gLite cli commands usage

Greetings

Some functionalities and even new tools have been added by the contributors below:

 *Mark Santcroos <M.A.Santcroos@amc.uva.nl>
  Created the lcg-rec-rep tool 

 *David O'Callaghan https://github.com/davidoc
  Added new options: dryrun, noclobber and up/download streams
  Added lcg-rec-lr
  He's also maintaining this code at: https://github.com/davidoc/lcg-rec-tools
 
 *Nikolaos Charitonidis <nikolaos.charitonidis@cern.ch>
  Early adopter/tester of the lcg-rec-tools 

More information are available at: http://gilda.ct.infn.it/wikimain?p_p_id=54_INSTANCE_t9W0&p_p_lifecycle=0&p_p_state=normal&p_p_mode=view&p_p_col_id=column-2&p_p_col_count=1&_54_INSTANCE_t9W0_struts_action=%2Fwiki_display%2Fview&_54_INSTANCE_t9W0_nodeName=Main&_54_INSTANCE_t9W0_title=Lcg-rec-tools



