---
title: Overview of Service Scheduling and Scheduling experience in Dynamics 365 Customer Service
description: This article provides information on the basics of service and service scheduling in Dynamics 365 Customer Service.
ms.date: 05/07/2024
author: lalexms
ms.author: laalexan
ms.topic: overview
---

# Overview of Service Scheduling

Avoid disruptions in service by making sure that your resources are scheduled optimally and efficiently. Using Scheduling in Customer Service Hub, you can plan and schedule service activities for your customers by bringing together all your resources.

## Prerequisites

Scheduling in Customer Service Hub is a [customer-driven update](scheduling-experience.md#set-up-scenarios). You need to avail and enable the service scheduling package, which also includes the Universal Resource Scheduling (URS) functionality.

## Understand the scheduling experience

Scheduling, which is built on top of URS, provides an efficient way to schedule resources for service activity. It considers the availability of employees, facilities, and equipment to plan schedules accordingly. It also helps customer service organizations with improved service quality by preventing over-scheduling.

### Scheduling scenario

The following scenario helps to understand how the scheduling capability lets you manage your service activities seamlessly:

Contoso bike repair schedules repair services for their customers. To facilitate this process, Contoso needs to bring together the following information:

- Geographical locations where they need to offer their services.
- The personnel and equipment they need to perform those services.
- The types of bike repair services they offer.
- Work hours during which they perform their services.
- Capacity and expert level for all personnel.

Contoso can benefit from the scheduling feature by quickly catering to their customers with their repair services. With the various scheduling entities, they can plan service activities for their customers by considering the availability of resources, facilities, and equipment.

Let's see how Contoso accomplishes the task:

**Step 1: Create organizational units**  </br>
   Organizational units are the locations where Contoso provides service to their customers. [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Create and manage organizational units](create-org-units-cs-scheduling.md)

   ![organizational units.](../media/org-unit-csh.png) 

**Step 2: Create resources**</br>
  Contoso lists the resources required to perform the services. 

  > [!NOTE]
  > You can create all resource types using the Resource entity.

  In this example, two resources (contacts) Bert Hair and Gilda Moss are created. Similarly, two more resources (facility/equipment) are created as Bike repair workbench - 1 and Bike repair workbench - 2, which are required to perform the service. [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Create and set up bookable resources](resources-service-scheduling.md)

  ![resouces-csh.](../media/resources-csh.png) 


**Step 3: Set work hours for the resource, resource group or facility/equipment** </br>
   The availability of the resources is defined in the work hours section. [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Set work hours for the resources](resources-service-scheduling.md#set-work-hours-for-the-resources)

   ![set-work-hours.](../media/set-work-hours-csh-1a.png)  
   
  
**Step 4: Create resource groups** </br>
   The resources are aligned in resource groups or resource categories. 

   In the example, Bert Hair and Gilda Moss are grouped as Technicians and Bike repair workbench - 1 and Bike repair workbench - 2 are grouped as Workbenches.
    
   [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Create and manage resource categories](resource-categories-service-scheduling.md)

   ![resource group.](../media/res-groups-csh.png) 


**Step 5: Create a service record**  </br>
   Contoso now collates all the above inputs to create a bike repair service record for the customer. They also specify the resources/resource groups they will need for the service. [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Create or edit a service in Service Scheduling](create-edit-service-csh.md)

   ![service record in Customer Service Hub.](../media/service-csh.png "service record in Customer Service Hub") 
 
**Step 6: Create a service activity**  </br>
   A service activity is defined to look for the next available time slot to schedule the service and align resources as per requirement.  [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Schedule a service activity](../use/schedule-service-activity-csh.md)

   ![service-activity.](../media/service-activity-csh.png)

**Step 7: Book the service in the schedule board**  </br>

  The schedule board displays all the service configurations at one place to quickly schedule a service. [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Use the schedule board to configure service activity](../use/use-schedule-board-configure-service-activity.md)

   ![schedule-board.](../media/schedule-board-csh.png)  

## Understand scheduling entities

Scheduling entities are grouped under the following logical groups:

**Scheduling**

- **Resources** </br>
   Anything that needs to be scheduled can be termed as **Resources**. This can be personnel, crews, service centers, company assets (equipment), accounts, or contacts. 

  [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Create and set up bookable resources](resources-service-scheduling.md)

- **Facilities/Equipment**  </br>
   Facilities and equipment are resources you'd use to perform services for your customers. Facilities can be physical spaces like service bays or conference rooms and equipment could be tools or other assets. 

   [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Add facilities and equipment to schedule service](add-facilities-equipment-ss-csh.md)

- **Resource Categories** </br>
   With Resource categories,  you can group your bookable resources by type. For example, you can create categories like technician, supervisor, subcontractor, vehicle, or equipment. 
 
   [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Create and manage resource categories](resource-categories-service-scheduling.md)

- **Services**  </br>
   To make scheduling services quick and easy, it's helpful to predefine the specifics of the services you'd provide to customers. 

   [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Create or edit a service](create-edit-service-csh.md)

- **Service Activities** </br>
   Create a service activity by finding the next time resources are available for a service. 

   [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Schedule a service activity](../use/schedule-service-activity-csh.md)

- **Fulfillment Preferences** </br>
    Choose and customize how to display schedule assistant results, like with neat hourly appointments or morning and afternoon time windows.

    [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Fulfillment preferences](../../common-scheduler/fulfillment-preferences.md)

**Tools**

- **Schedule Board** </br>
   The Dynamics 365 Customer Service schedule board provides an overview of resource availability and bookings you can make. 

   [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Use the schedule board to configure service activity](../use/use-schedule-board-configure-service-activity.md)

**Settings**

- **Organizational Units** </br>
   Your company organizes its business by geography, function, or other areas. You can create organizational units that reflect your business. 

   [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Create and manage organizational units](create-org-units-cs-scheduling.md)

- **Business Closure** </br>
   Prevent scheduling resources on holidays and other non-working days by defining business closures. 

   [!INCLUDE[proc_more_information](../../includes/proc-more-information.md)] [Set when your business is closed](../use/set-when-business-closed-csh.md)


### See also    
    
[Set up the Service Scheduling experience](scheduling-experience.md)  
[Access scheduling in the Customer Service Hub and Customer Service workspace](access-scheduling.md)  
[Install Service Scheduling from Power Platform](install-service-scheduling-from-power-platform.md)  
[Service Scheduling FAQ](service-scheduling-faq.md) 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
