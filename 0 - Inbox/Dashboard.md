## **Daily Notes to Atomize:**
%% List the files in 1- daily notes that are marked as to-do %%
```dataview
table from "1 - Daily Notes" and (#To-Do and !#Completed)
where file.name != "Dashboard"
```

## **Atomized Notes in Progress:**
```dataview
table from "3 - Slip-Box" and (#To-Do)
```

## **Incomplete Daily Tasks:**
```dataview
task from "1 - Daily Notes"
where !completed
```