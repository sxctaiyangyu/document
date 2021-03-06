# EnSaaS-K8s-Service 4.0.2- (2020-03-10)

## Summary Update

Added:

- Platform management：
  - Add workload page，user can view the workload of the namespace.
  - Add real-time log of workload pod.

Updated:

- Add categories in the left menu bar to distinguish between the dedicated cluster and shared cluster.

Fixed:

- Fix the issue of viewing resources by subscription.
- application page cannot be displayed.


- when create WS failed, ws record will exist in the database.Bug12493.


- when getting resource of WS return return value  . Bug 12465.
- Fixed the permissions of datacenteradmin under the default subscription.
- The authority of WS owner in clusteragent.
- when input the wrong subscription number,user can still get the the workspace name according to the workspace ID. Bug 12459.
- Optimize API error messages.
- When switching the subscription number on the node page, the node list is not updated in time,  still displays the node information obtained last time.
- From General workspace switch to NS list page and go back to the previous page. The add workspace button will appear.





# EnSaaS-K8s-Service 4.0.0- (2020-02-19)

## Summary Update

Added:

- Subscription  and user permissions:
  - Add subscription name on the top navigation bar, and support  display resources by the subscription name
  - Users with subscription privileges (subscription admin/user) can see and manipulate the resources purchased by the subscription

- Monitor:
  - Integrate RMS : Provide different levels of monitoring display



Fixed:

- Modify the synchronization method of rolebinding between MP and sso, and add subscription number verification before creating rolebinding.
- Add synchronization mechanism between slave cluster and master cluster to fix the problem that info and metric cannot be updated immediately 
- Fix port error when clusteragent synchronizes resources to master cluster
- In the applications page,  only 20 app can be displayed 
- On the workspace overview page, the limitmemory of the quota is error
- Click console from SSO UI, unable to log in MP automatically
- workspace owner and namespace developer in namespace page. After the cluster is switched through the breadcrumbs, the workspace overview page displays n / A, and cannot resume though refresh
- User with namespace developer permission. when entering the namespace page for the first time or refreshing the page, the workspace drop-down box does not support clicking
- When the namespace developer enters the application page, the workspace drop-down box cannot get the workspace list. and refresh this page, the namespace list is  empty
- In scale namespace quota page, the page display nothing when change the quota of namespace
- Modify page scaling problem
- Fix when the user has multiple permissions, the UI display error.

