graph LR

    subgraph Planning
        Plan[Plan 'Tool Name']
    end

    subgraph Development
        Code[Code 'Tool Name']
        Build[Build 'Tool Name']
        Test[Test 'Tool Name']
    end

    subgraph Deployment
        Release[Release 'Tool Name']
        Deploy[Deploy 'Tool Name']
    end

    subgraph Operations
        Operate[Operate 'Tool Name']
        Monitor[Monitor 'Tool Name']
    end

    Plan --> Code
    Code --> Build
    Build --> Test
    Test --> Release
    Release --> Deploy
    Deploy --> Operate
    Operate --> Monitor
    Monitor --> Plan

