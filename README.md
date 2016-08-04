# LiteWorkflow
Lightweight event driven workflow execution engine.

## Core concepts  

**Workflow** static workflow definition   
**WorkflowPhase** static workflow state representation   
**WorkflowAction** called by specific event handler at specific lifycycle. Notification, Approval are both as actions
**WorkflowTransition** extends from WorkflowAction  
**WorkflowExecution** An instance for workflow running  
**ExecutionContext** running context to relate data and state transfer between whole execution lifecycle  
**Event** workflow execution lifecycle event such as **WorkflowStartingEvent**, **WorkflowStartedEvent**, **WorkflowPhaseEnteringEvent**, **WorkflowPhaseEnteredEvent**  
**EventBus** event pub sub system to decouple workflow action handler.
