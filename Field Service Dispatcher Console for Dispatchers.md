## Where Does the Dispatcher Fit In?
On a typical day, a dispatcher has a lot to do.

- Monitor service appointments in the assigned service area.
- Reschedule or cancel service appointments.
- Reassign service appointments to nearby mobile workers when the situation changes.
- Optimize the schedule based on worker skills, location, availability, and job priority.
- Keep mobile workers busy by managing their schedules.
- Coordinate resources, back office, and warehouse services.
- Dispatch service appointments to third-party contractors and crews and track them to completion.
Much of this work is done by the scheduling engine, but dispatchers monitor everything to make sure that the scheduled plan becomes a reality.

The dispatcher console includes:
- Appointment list
- Easy-to-reach scheduling actions
- Dynamic Gantt chart
- Interactive map
- Other nifty features.
You can customize all kinds of things.
- The time horizon
- The dates displayed
- Gantt and map display preferences
- Color schemes
- Data filters

# Explore the Dispatcher Console

![[Pasted image 20240103123230.png]]

- **Policy (1).** Choose the policy Field Service uses to schedule appointments. Right now, Ursa Major is using a Customer First scheduling policy. Jacinta can change it if Ursa Major’s needs change, such as during an emergency.
- ![Territories icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/explore-the-dispatcher-console/images/bf03067783b3f76f67ac371f94803c6a_territories.png) **(2)**. Use to select the service territories to display appointments not associated with a service territory. Jacinta always displays her home territory of Los Angeles. When she’s helping out in Denver, she also displays that territory.
- ![Settings icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/explore-the-dispatcher-console/images/5deaea1e285d26fcd8cd3b48d9c9dd4a_settings-2.png) **(3)**. Use to customize the appearance of the appointment list, such as appointments per page.
- **Time frame (4).** Jacinta’s appointment list matches the Gantt. She can choose different types of dates to display or set a time horizon.
- **Service appointments displayed (5).** Jacinta is viewing all service appointments, but she can filter them, such as viewing only unscheduled appointments. If she doesn’t see the filter that she needs, she can create a custom one.
- **Actions for selected appointments (6).** If Jacinta selects one or more appointments, she can choose to schedule, dispatch, flag, unflag, or optimize them.

## Check Out the Gantt Schedule
![[Pasted image 20240103123524.png]]

- Assess the health of your schedule at a glance by checking the **key performance indicator (KPI) bar (1)** in the top right. The bar shows stats like total scheduled time, average travel time per appointment, and the number of appointments that are in jeopardy.
- Use the ![Filter icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/explore-the-dispatcher-console/images/847c0f449048f1457959a1d18a8e9f5f_filter.png) **(2)** at the top of the Gantt to **filter** which mobile workers and records appear on the Gantt. For example, filter mobile workers by skill or resource type. From the filter, you can also control which hours of the day are shown, apply a custom color scheme, and customize the long-term and utilization views.
- Control the **time frame (3)** using the arrows and calendar.
- The **resource list (4)** shows mobile workers organized by territory. Since Jacinta is looking at Los Angeles, there’s Ursa Major’s star installer, James Clifton. You can display custom text under a mobile worker using the Gantt Label field. James would like Jacinta to put Installation Wizard under his name, but for now it just says Installation Expert.
- The **schedule view (5)** at the center shows appointments, absences, breaks, travel times, and service crew assignments. Jacinta uses Gantt keyboard shortcuts to view records and navigate the schedule view.
## Bring Up Maps
- In the Gantt, click **Map**.
- Click **Traffic**.

# Customize Your View

## Change the Time Horizon

1. From the App Launcher, find and select **Field Service** to open the dispatcher console.
2. In the service appointment list, click ![Settings icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/customize-your-view/images/5deaea1e285d26fcd8cd3b48d9c9dd4a_settings-2-2.png) and select **Dispatch Console Settings**.
3. For the Scheduling window length, enter the time horizon. Jacinta enters `3`.
4. Click **Save**.
5. Click ![Horizon fields icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/customize-your-view/images/46c5e2f868cbe544ee2dfcd16603c128_horizon-field.png), and select the fields to fall into your time horizon. Jacinta selects **Due Date**, **Scheduled Start**, and **Scheduled End**.
6. Next to Horizon, select today’s date.  
    ![Service appointments with the horizon fields menu opened.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/customize-your-view/images/3556b393dcdefe9012167ed324e92a8c_manage-service-appt-1.png)

## Show More Days on the Gantt

![Gantt with options for changing the date and number of days to display.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/customize-your-view/images/3f2f642e23aa05838a5ec69d854f134d_manage-gantt-1.png)

- **The date displayed in the Gantt (1)**—Usually, Jacinta views today’s schedule, but sometimes she skips back a day or two to see more context.
- **Ways to set the day displayed (2)**—Use the arrows to move forward or backward a day at a time. Use the calendar to select a date to view.
- **Ways to change what is displayed in the Gantt (3)**—Jacinta usually displays two days at a time to get a better scope of how changes affect her schedule.

![[Pasted image 20240103125659.png]]

## Adjust the Gantt’s Color Palette
She decides to create a custom color palette for her Gantt based on the appointment due date.

1. In the dispatcher console, click the filter icon at the top of the Gantt.
2. Click the **Palettes** tab.
3. Click **Open palette editor**.  
    ![Filter icon menu opened displaying Palettes tab.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/customize-your-view/images/898ec34c5f7ce10a65b94abd247546fc_manage-gantt-3.png)
4. Click **New Palette**.
5. Enter a name and description. Jacinta enters `Due Date Approaching`.
6. Select the field on which to base the palette. Jacinta selects **Due Date**.
7. Define the color spectrum. Jacinta is using a picklist field, so she assigns a color to each picklist value. Here’s what she uses.
    - Minimum Value: `0` days
    - Minimum Value Color: `#ff0000`
    - Maximum Value: `7` days
    - Maximum Value Color: `#ffff00`
    - No value: `#40bfbd`
    - Number of Colors: `**7**   `**Tip:** We recommend creating a high-contrast spectrum to assist users with color vision difficulties.
8. Select **Active** to make the palette available to dispatchers.
9. Click **Save**.
# Manage Service Appointments

## Schedule Appointments
1. In the appointment list, click an unscheduled appointment to display more information.
2. Click **Schedule**.
## Fix Rule Violations
A rule violation occurs when the service appointment isn’t following the scheduling rules in the scheduling policy you’ve selected. 
For example, an appointment scheduled to a resource without a required skill or an appointment scheduled before the earliest allowed start date are both rule violations.
![[Pasted image 20240103133326.png]]

## Dispatch Appointments
Sometimes, the schedule changes after an appointment is already dispatched. Jacinta hates it when that happens, but it’s unavoidable. But that’s OK. 

The dispatcher just changes the appointment and notifies the mobile worker. The mobile worker changes their plans and works on their new appointment. 

If one appointment changes, later appointments in that mobile worker’s schedule may need to be rescheduled and redispatched, too.

# Handle the Unexpected

## What If Someone Calls in Sick?

First, she creates an absence for James.

1. From the App Launcher, find and select **Field Service**, then click the **Field Service** tab to open the dispatcher console.
2. In the Gantt, hover over the absence dropdown to view the up and down arrows and the tooltip.
3. Use the arrows to set the duration of the absence in minutes. Jacinta selects **300** because that’s how many minutes are in 5 hours. ![The absence icon showing 300 minutes selected.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/handle-the-unexpected/images/1a45479ce402878681308187e759aa02_unexpected-dispatcher-absence-1.png)
4. To set the reason for the absence and the label to display on the Gantt, click the arrow on the right. Jacinta chooses **Medical** and enters `Out sick`. ![The absence icon showing Medical and Out sick for Default Non Availability.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/handle-the-unexpected/images/3246f22888ae054f51985c3a4f6c2b89_unexpected-dispatcher-absence-2.png)
5. Drag the absence dropdown to the location of the absence on the Gantt. Jacinta drags the absence to James Clifton at noon. The absence appears on the Gantt. ![Absence showing next to James Clifton’s name.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/handle-the-unexpected/images/634160fff66fabc267024ba627837262_unexpected-dispatcher-absence-3.png)

Now, Jacinta must reschedule James Clifton’s remaining appointments for today.

1. Right-click the appointment and select **Reschedule**. ![Right click menu opened over James Clifton’s appointment with Reschedule selected.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/handle-the-unexpected/images/c62a0b65486ca43feb313cde138007ab_unexpected-dispatcher-absence-4.png)
2. Repeat for the other appointments.

## Handle an Emergency
1. From the App Launcher, find and select **Field Service**, then click the **Field Service** tab to open the dispatcher console.
2. In the service appointment list, click the emergency appointment to view more details.
3. Click the **Parent Record ID**.
4. In the Feed tab, click **Emergency**, then **Emergency Dispatch**.![Emergency tab in the Feed.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/handle-the-unexpected/images/a655c686ac7b08d3828f96720472d651_unexpected-emergency-1.png) The dispatcher console displays the closest available mobile workers who can help Violet. It's James Clifton and he's 21 minutes away.![Map showing the closest candidates with James Clifton selected.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/handle-the-unexpected/images/53d973a35d5712f9429f499701b9ba04_1654107025961.png)
5. Click **Dispatch**, then **Confirm and Dispatch**.

## Use a Polygon to Add a Service Area

[Enable Field polygon](https://help.salesforce.com/s/articleView?id=sf.pfs_map_polygons_enable.htm&type=5)

1. In the dispatcher console, click **Map**.
2. Zoom in until you can comfortably see the boundaries.
3. Click **Map Layers**.
4. Select **Polygons**.
5. Click **New**.
6. Name your polygon and select a color. Jacinta names her polygon `Century City` and chooses bright blue as the color.
7. Select the larger service territory. Jacinta selects **Los Angeles**.
8. Before you can save it, you must draw your polygon on the map.
    - Jacinta clicks the first border at Century Park West and Santa Monica Boulevard.
    - She clicks the second border at Century Park West and Pico Boulevard.
    - She clicks the third border at Pico Boulevard and Century Park East.
    - And, she finishes up with the fourth border at Century Park East and Santa Monica Boulevard.
9. ![Map showing the newly created service territory.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/field-service-dispatcher-console-for-dispatchers/handle-the-unexpected/images/669e943f6d0e3ad7a85151b80fd8ef7c_unexpected-dispatcher-polygon.png)
10. Click **Save**.