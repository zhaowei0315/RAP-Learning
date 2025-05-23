# RAP-Learning
RAP Learning - source code

## ABAP RESTful Application Programming Model (RAP)   
https://youtu.be/iXYlD_xtQ68?si=Ai-SBDK-l0o4i-WC  
https://www.bilibili.com/video/BV1oVN3ehEbN?spm_id_from=333.788.videopod.episodes&vd_source=315e38f363cf6dd7b4dcf1f16f823f47  


## Generate SM30 - Create Business Configuration Maintenance Object  
https://developers.sap.com/tutorials/abap-environment-business-configuration-object..html  

### All tables (Business Configuration Maintenance Object) must fulfill the following requirements:  
#### have a client key field
#### have delivery class C
#### allow data maintenance
#### (optional) have a timestamp field with data element ABP_LOCINST_LASTCHANGE_TSTMPL. If the table doesn't contain this field, the concurrency control is not active
##### local_last_changed_at : abp_locinst_lastchange_tstmpl;
#### have a timestamp field with data element ABP_LASTCHANGE_TSTMPL. If the table doesn't contain this field, the entire ETag is handled by CDS entity I_CstmBizConfignLastChgd
##### last_changed_at       : abp_lastchange_tstmpl;
#### key fields use domain for character-like
