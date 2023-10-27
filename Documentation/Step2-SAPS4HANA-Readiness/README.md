## Check SAP S/4HANA Readiness
In this section, you will activate the APIs related to SAP Environment, Health and Safety for this scenario.

### Activate the API_EHS_REPORT_INCIDENT_SRV Service

1. In your SAP S/4HANA GUI system, open the **/n/IWFND/MAINT_SERVICE** transaction.

2. Activate the **API_EHS_REPORT_INCIDENT_SRV** service.

    ![plot](./images/s4EHS-service.png)

Creating a **EHS Incident Safety Observation**  requires two roles 
```
- SAP_BR_INDUSTRIAL_HYGIENIST
- SAP_EHSM_HSS_INCIDENT_MANAGER
```

Make sure to add these roles. To add these roles, in your SAP S/4HANA GUI system, 

1. Open the **/n/su01** transaction in SAP S/4HANA.

2. Find the SAP S/4HANA user you want to add the roles to and Press Enter.

3. Click the **Roles** Tab and Choose the **Edit** Option.

4. Add the above two roles and **Save** the changes


Based on your business scenario, expose the respective APIs (For example, Record Safety Observation, Report Incident etc.).

In the next step, you can choose to either setup cloud connector or SAP Private Link Service based on the SAP S/4HANA installation.
