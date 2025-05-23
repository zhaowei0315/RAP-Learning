# RAP-Learning
RAP Learning - source code

## ABAP RESTful Application Programming Model (RAP)   
https://youtu.be/iXYlD_xtQ68?si=Ai-SBDK-l0o4i-WC  
https://www.bilibili.com/video/BV1oVN3ehEbN?spm_id_from=333.788.videopod.episodes&vd_source=315e38f363cf6dd7b4dcf1f16f823f47  


## Generate SM30 - Create Business Configuration Maintenance Object  
https://developers.sap.com/group.abap-env-factory.html    

### All tables must fulfill the following requirements:  
#### 1.Have a client key field
  -- key client            : abap.clnt not null;
#### 2.Key fields use data element and domain for character-like
#### 3.Have delivery class C
##### @AbapCatalog.deliveryClass : #C
#### 4.Allow data maintenance
##### @AbapCatalog.dataMaintenance : #ALLOWED
#### 5.(optional) Have a timestamp field with data element ABP_LOCINST_LASTCHANGE_TSTMPL. If the table doesn't contain this field, the concurrency control is not active
  -- local_last_changed_at : abp_locinst_lastchange_tstmpl;
#### 6.Have a timestamp field with data element ABP_LASTCHANGE_TSTMPL. If the table doesn't contain this field, the entire ETag is handled by CDS entity I_CstmBizConfignLastChgd
  -- last_changed_at       : abp_lastchange_tstmpl;

