# scheduler

Scheduler is a one-script, dependencyless module to schedule tasks, known as "systems".

## Example Init

```lua
local SchedulerClass = require(path.to.scheduler)
local Scheduler = SchedulerClass.new("Test")

local Runtimes = {
    "PreRender",
    "RenderStepped",
    "Heartbeat"
}

local System = require(path.to.system)

Scheduler:AddSystem(System)
Scheduler:SetRuntimes(Runtimes)

Scheduler:Start()
```

## Example System

```lua
local System = {}

System.Configuration = {}
System.StepMode = "PreRender"

function System:Init()
    --runs once
end

function System:Step()
    -- This runs every frame!
end

return System
```
