## Instrument Kubernetes with Dynatrace - Part 2

This lab guide will deploy Dynatrace integration for Kubernetes.

### Update Kubernetes Integration Settings

1. In Dynatrace Tenant, Click Settings -> Cloud and Virtualization -> edit icon for configured K8s cluster

   ![K8SConfig](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/011_k8sUI.png)    

3. Toggle the following switches:
   - Change the connection name to "HoT 2021".

   - Toggle OFF "Require valid certificates for communication with API server" (this workshop cluster uses self-signed).

   - Toggle ON "Monitor Prometheus exports"
   
   ![K8SToggles](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/012_k8sSlider.png)

4. Click Add event field selector

   ![K8SEventSelector](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/013_k8sEvents.png)

5. Provide a field selector (other events) name and expression (involvedObject.kind!=Node)

   ![K8SEventSelector](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/014_k8sEventsS.png)

6. Toggle on Monitor events

   ![K8SMonitorEvents](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/015_k8sUISave.png)
   
   - Click Save. 

7. Verify Dynatrace Operator Deployment
   
   - Navigate to Kubernetes -> HoT 2021 
   - Scroll down to Name Spaces and select Dynatrace
   
   ![K8SVerifyDT](/Dynatrace%20for%20Cloud%20Operators%20(K8s)/assets/images/016_VerifyDT.png)
