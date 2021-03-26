Config_STG.sql
>> DEFINE MIGRATE_VAL_FROM_PRIME3 = 1

Config_UAT.sql
>> DEFINE MIGRATE_VAL_FROM_PRIME3 = 0

-------------------------------------------------------

Patch_Script.sql
>> 
If (:usemigvalue=0) Then 
	Update xxx config; 
End If;