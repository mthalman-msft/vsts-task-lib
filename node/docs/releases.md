# VSTS-TASK-LIB RELEASES

## 0.8.2
  * Pattern change.  Use async function with code in try/catch.  SetResult to fail in the catch.  See samples.
  * setResult will not halt execution.  Process.exit caused output loss in some scenarios.
  * All GetInput functions will throw if required and not supplied
  * Disk operations will throw if they fail
  * mv and cp take options string as optional arg
  
## 0.7.3
 * Updated `setResult` to log the message as an error issue if the result is Failed.

## 0.7.2
 * Updated `getDelimitedInput` to remove empty entries.

## 0.7.1
 * Updated `ToolRunner` to emit lines.
 * Fixed initialization so that `.taskkey` file is not left in the repo root.

## 0.7.0
 * Updated `ToolRunner.arg` to simply append to the arg array that is passed to `spawn`.
 * Added `ToolRunner.argString` to split additional arguments, which are then appended to the arg array that is passed to `spawn`.
