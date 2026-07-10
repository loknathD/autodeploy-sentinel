# User Flow

1. User logs in.
2. User creates a project.
3. User connects a Kubernetes cluster.
4. AutoDeploy Sentinel validates connectivity.
5. User selects a namespace.
6. User selects a workload or pod.
7. User clicks Analyze.
8. Backend collects:
   - Pod details
   - Events
   - Logs
   - Deployment configuration
9. AI analyzes the collected context.
10. User receives:
    - Root cause
    - Confidence score
    - Recommended fixes
    - Suggested kubectl commands