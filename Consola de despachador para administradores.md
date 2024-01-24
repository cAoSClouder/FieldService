# [Configurar la consola de despachador](https://trailhead.salesforce.com/es-MX/content/learn/modules/dispatcher-console-for-admins/set-up-the-dispatcher-console)
## Make It Your Own

Maria tells them the kinds of things they can change.

- **Admin settings.** These settings control the nuts and bolts of Field Service. 
	- Use them to define:
		- The lifecycle of a service appointment
		- Customize global actions
		- Set up scheduling and optimization policies and more. 
		- You can also customize how a dispatcher works in the Gantt, such as by setting the timezone displayed. 
		- You can determine how often the Gantt is refreshed, display absences, and much more.
	
- **Customize field sets.** Field sets determine which fields are displayed or used for filtering in the Gantt. Add or remove fields from the field sets to see just the fields that your dispatchers need.

- **Custom filters.** Enable custom filters, then create filters for the service appointments picklist.

- **Custom icons for the Gantt.** Add custom icons to service appointments on the Gantt and the map.

- **Custom actions.** Add custom actions to the Gantt. Custom actions can either call an Apex class or open a Visualforce page, and can be run on records in several areas of the dispatcher console. To keep the dispatcher console tidy, actions are shown in dropdown action lists with icons.

# Customize Dispatcher Console Settings
## Change the Time Zone Displayed
(Solo si se tienen varios horarios en un pais)
Maria tells her it’s not a problem to set this up for her.

1. From the App Launcher ![App Launcher icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/customize-dispatcher-console-settings/images/fafce66bd90f5afcc38b93b18305729e_app-launcher-icon-2.png), find and select **Field Service Admin**.
2. Click **Field Service Settings**.
3. Open **Dispatcher Console UI** and click **Gantt Configurations**.
4. From Gantt chart timezone, select **Territory Timezone** to display appointments in the time zone used by the territory. ![Dispatcher Console UI settings showing Territory Timezone selected.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/customize-dispatcher-console-settings/images/999cccd589296b368a167b73791e679c_times-fields-1.png)
5. Click **Save**.
## Add and Remove Fields with Field Sets

Maria adds the new field.

1. Click ![Setup](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/customize-dispatcher-console-settings/images/53883122f709cd0cabf9c39044235731_setup.png), then select **Setup**.
2. Click **Object Manager**.
3. Click **Service Resource**..
4. Click **Field Sets**.
5. Click **Resource Lightbox**.
6. Drag the **Efficiency** field onto the layout. ![Object Manager showing the Efficiency field being dragged into the Resource Lightbox field set.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/customize-dispatcher-console-settings/images/f9880ce61322730e77a18081fbbee6f9_times-fields-2.png)
7. Click **Save**.

## Activar la programación de alimentación paulatina
Cuando esta se activa, los trabajadores móviles no reciben su nueva cita hasta que completan la actual. 
Esto resulta útil para las compañías que trabajan con citas que se mueven mucho durante el día.

1. From the App Launcher ![App Launcher icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/customize-dispatcher-console-settings/images/fafce66bd90f5afcc38b93b18305729e_app-launcher-icon-4.png), find and select **Field Service Admin**.
2. Click the **Field Service Settings** tab.
3. Open **Dispatch** and click **Drip Feed**.
4. Select **Enable Drip Feed Dispatching**.
5. Select the number of appointments to dispatch. Maria selects **1**. ![Dispatcher Console with drip feed dispatching enabled.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/customize-dispatcher-console-settings/images/893659a488169918d36645ca98dfe5fe_times-fields-4.png)
6. Click **Save**.

# Agregar filtros e iconos personalizados
## Activar filtros personalizados
Los filtros existentes, como Unscheduled (Sin programar) o In Jeopardy (En riesgo), porque le muestran sus prioridades inmediatas.

Before Jacinta can create any filters, Maria must enable them.

1. From the App Launcher ![App Launcher icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/add-custom-filters-and-icons/images/fafce66bd90f5afcc38b93b18305729e_app-launcher-icon-5.png), find and select **Field Service Admin**.
2. Click the **Field Service Settings** tab.
3. Click **Dispatcher Console UI** and select **Enable Custom Filters**.


## Create a Custom Filter
Filtro que muestre únicamente las citas que tardan varias horas en completarse

1. From the App Launcher ![App Launcher icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/add-custom-filters-and-icons/images/fafce66bd90f5afcc38b93b18305729e_app-launcher-icon-6.png), find and select **Field Service**, then click the **Field Service** tab.
2. To the right of the filter picklist, click ![Filter](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/add-custom-filters-and-icons/images/59a32961a63063560c4e9c2df32d8f12_new-filter.png) and select **New**.
3. Enter the name, description, and dates to select. Jacinta enters the following.
    - Name: `Long Jobs`
    - Description: `Show jobs longer than 4 hours`
    - Date Selection: Jacinta enters `3` for the number of days before and after the selected horizon date. The filter displays only appointments that fall within that date range.
4. Set the field criteria. Jacinta sets criteria for two fields.
    - Jacinta sets the first field criteria. She chooses **Duration** as the field, **greater or equal** as the operator, and **4** as the value. That’s for jobs that take more than 4 hours.
    - Jacinta sets the second field criteria. She chooses **Status** as the field, **does not contain** as the operator, and **Completed** as the value. She doesn’t want to see jobs that are already completed, just jobs left to do.![Filter Editor displaying the field criteria for Duration and Status.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/add-custom-filters-and-icons/images/810abf96943bc8202b70cd71b4a2b018_filters-icons-1.png)
5. Choose the fields to display. Jacinta wants to display the default fields in the Service Appointment List Columns field set, so she leaves it blank.
6. Decide whether to share the filter with other dispatchers. Jacinta wants to share, so she selects **Make this filter available to all users**.
7. Click **Save**.

- Select the custom filter in the filter picklist. Jacinta selects **Long Jobs**.
- Click ![Filter](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/add-custom-filters-and-icons/images/59a32961a63063560c4e9c2df32d8f12_new-filter-2.png)and choose the desired option.
 ![[Pasted image 20240103194043.png]]

## Add a Custom Icon to the Gantt
First, Maria must add the Gantt icon field to the page layout for service appointments so Jacinta can see it on the Gantt.

1. Click ![Setup](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/add-custom-filters-and-icons/images/53883122f709cd0cabf9c39044235731_setup-5-2.png) then select **Setup**.
2. Click **Object Manager**.
3. Click **Service Appointment**, then click **Field Sets**.
4. Click **Service Lightbox**.
5. Drag the **Gantt Icon** field to the **In the Field Set** section.![](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/add-custom-filters-and-icons/images/637dd38c9fbe1f325d827b6966b78aef_console.jpg)
6. Click **Save**.

Maria checks to make sure that the new field displays properly. If you try these steps in your org and can't see the Gantt icon field, make sure that you've [assigned the page layout](https://help.salesforce.com/articleView?id=customize_layoutassign.htm&type=5) you changed to the correct user profiles.

Jacinta is ready to add her icon to a deserving service appointment.

1. In the Gantt, right-click the service appointment and choose **Details**. Jacinta right-clicks James Clifton's first appointment.
2. In the Details tab, click **Edit**.
3. Enter the icon URL in Gantt icon. Jacinta enters [`https://www.salesforce.com/news/wp-content/uploads/sites/3/2021/05/Salesforce-logo.jpg?resize=1536,864`](https://www.salesforce.com/news/wp-content/uploads/sites/3/2021/05/Salesforce-logo.jpg?resize=1536,864).
4. Click **Save Changes** and close the tabs.
5. Refresh the Gantt to view the icon. (Your screen may not look exactly like this screenshot.)![Gantt showing a sunshine icon next to James Clifton’s first appointment.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/dispatcher-console-for-admins/add-custom-filters-and-icons/images/98f7a263951d5e2e32b883638749764b_filters-icons-4.png)
# Add a Custom Action
## Escribir una clase Apex
[Guía de desarrollador de Field Service](https://developer.salesforce.com/docs/atlas.en-us.220.0.field_service_dev.meta/field_service_dev/fsl_dev_code_samples_dispatcher.htm?_ga=2.211650198.22009853.1704200319-803831644.1702566254)
