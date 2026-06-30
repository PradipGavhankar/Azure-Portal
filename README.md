# Azure-Portal
# Azure Access Verification Methods

Before starting work in an Azure environment, it is essential to verify that you have the correct permissions and role assignments. Below are two standard methods to check your Azure rights.

---

## Method 1: Check via Subscription Access Control (IAM)
This method allows you to verify your access directly from the specific subscription you intend to work on.

### Step-by-Step Verification:
1. Log in to the **Azure Portal**.
2. Search for and select **Subscriptions** from the top search bar or the left sidebar.
3. Select the target subscription (e.g., `Azure subscription 1`).
4. In the left-hand navigation menu for that subscription, click on **Access control (IAM)**.
5. Click on the **View my access** tab.
6. Here, you will see your explicit role assignments and inherited permissions for this specific subscription.

### Visual Reference:
![Azure Rights Check Method 1](./Snaps/AzRights%20Method%201.png)

---

## Method 2: Check via User Profile Role Assignments
This method allows you to view all role assignments mapped specifically to your user identity across the directory.

### Step-by-Step Verification:
1. Navigate to **All services** or search for **Users** in the main Azure search bar.
2. Search for and select your user profile (e.g., `Pradip Kumar`).
3. In the user profile's left navigation blade, click on **Azure role assignments**.
4. Review your assigned roles under the specific scope.

### Visual Reference:
As shown in the configuration capture below, navigating to the individual user profile confirms the active subscription-level access:

![Azure Rights Check Method 2](./Snaps/AzRights%20Method%202.png)


## Method 3: Check via Privileged identity Management >My role

> **Verification Details Confirmed in Image:**
> * **Scope:** `Azure subscription 1` (Subscription Level)
> * **Assigned Role:** `Contributor` (Provides full access to manage all resources, but does not allow assigning roles in Azure RBAC).
> * **Assigned To:** Explicitly mapped or via Group (`B18_G2`).
### Visual Reference:
![Azure Rights Check Method 3](./Snaps/AzRights%20Method%203.png)
