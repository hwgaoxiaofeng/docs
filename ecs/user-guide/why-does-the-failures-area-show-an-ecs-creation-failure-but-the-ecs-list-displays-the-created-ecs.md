# Why Does the  **Failures**  Area Show an ECS Creation Failure But the ECS List Displays the Created ECS?<a name="EN-US_TOPIC_0039524582"></a>

## Symptom<a name="section6720837161158"></a>

After you created an ECS bound with an EIP on the management console, the ECS creation was successful but binding the EIP failed due to insufficient EIPs. Although the  **Failures**  area showed that the ECS creation failed, the ECS was displayed in the ECS list. The results of the ECS creation task were inconsistent.

## Root Cause<a name="section26118472161749"></a>

-   The ECS list displays created ECSs.
-   The  **Failures**  area shows the ECS creation status, including the statuses of subtasks, such as creating ECS resources and binding an EIP. Only when all subtasks are successful, the ECS is created.

If the ECS is created but EIP binding failed, the task failed. However, the ECS you created is temporarily displayed in the list. After the system rolls back, the ECS is removed from the list.

