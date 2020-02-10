# jetbrains speedy shortcuts
on linux move files from folders to jetbrains config folder:
options/* -> ~/.PhpStorm2018.1\config\options <br />
tools/* -> ~/.PhpStorm2018.1\config\tools <br />
keymaps/* -> ~/.PhpStorm2018.1\config\keymaps <br />

(trying more elegant solution with symlinks [here in leazy](https://github.com/michondr/leazy/blob/driveto-setup/tasks/programs/jetbrains/doJetbrains.sh))
## keymap
### content (current window) actions
`ctrl w` - close tab (CloseContent) <br />
`ctrl shift t` - reopen closed tab (ReopenClosedTab) <br />
`ctrl shift w` - close all balast and keep current tab (CloseAllEditorsButActive) <br />

### git actions <br />
`alt w` - commit (CheckinProject) <br />
`alt e` - push (Vcs.Push) <br />
`alt r` - rebase (Git.Rebase) <br />
`altGraph a` - annotate (Annotate) <br/>
`altGraph s` - show git history of file (Vcs.ShowTabbedFileHistory) <br/>
`altGraph c` - compare with branch on git (Git.CompareWithBranch)<br />
`alt shift h` - show git commit history (Vcs.ShowTabbedFileHistory) <br />

### window actions <br />
`alt 1 (alt +)` - open/close project tree (ActivateProjectToolWindow) <br />
`alt 2 (alt ě)` - open/close database window (ActivateDatabaseToolWindow) <br />
`alt 3 (alt š)` - open/close open run window, usually with test results (ActivateRunToolWindow) <br />
`alt 4 (alt č)` - open/close remote host (ActivateRemoteHostToolWindow) <br />
`ctrl alt shift c` - copy filename while in project tree (CopyReferencePopup) <br />

### navigation <br />
`alt left (mouse back)` - Back <br />
`alt right (mouse forward)` - Forward <br />
`ctrl tab` - next tab (NextTab) <br />
`ctrl shift tab` - previous tab (PreviousTab) <br />
`ctrl alt left` - split tab to left (SplitVertically) <br />
`ctrl alt right` - split tab down (SplitHorizontally) <br />
`alt m` - next split screen (NextSplitter) <br />
`alt n` - previous split screen (PrevSplitter) <br />
`ctrl g` - go to row <br />
`ctrl e` - recent files <br />

### code tweaks <br />
`ctrl r` - refactor. works on methods, fields, classes, files. In project window can copy, move or rename files (Refactorings.QuickListPopupAction) <br />
`ctrl b (ctrl left click)` - jump to source. User to find source of method, or usages when in source <br />
`ctrl shift c` - comment whole line (CommentByLineComment) <br />
`ctrl x` - delete this line (or delete and copy selection) <br />
`alt h` - show local history (LocalHistory) <br />
`alt shift right (tab)` - move block of code 1 indent right (EditorIndentLineOrSelection) <br />
`alt shift left (shift tab)` - move block of code 1 indent left (EditorUnindentSelection) <br />
`alt up` - expand selection (EditorSelectWord) <br />
`alt down` - narrow selection (EditorUnSelectWord) <br />
`altGraph j` - join lines (EditorJoinLines) <br/>
`ctrl p` - show method parameters/arguments. an cycle though markdown view styles <br />

### code collapsing/expanding
`ctrl wheel-up` - collapse region (CollapseRegion) <br />
`ctrl shift wheel-up` - collapse all regions (CollapseAllRegions) <br />
`ctrl wheel-down` - expand region (ExpandRegion) <br />
`ctrl shift wheel-down` - expand all regions (ExpandAllRegions) <br />

### database actions <br />
`alt a` - dump current database table result to clipboard - this uses default/set dump-style (Console.TableResult.Copy.DumpToClipboard) <br />
`alt shift a` - dump current database table result  to file - this uses default/set dump-style (Console.TableResult.Copy.DumpToFile) <br />
`alt c` - count rows - works in database window, or when table view (Console.TableResult.CountRows) <br />
`alt d` - filter - works like adding a where cause (Console.TableResult.EditFilterCriteria) <br />
`alt p` - transpose (Console.TableResult.Transpose) <br />
`ctrl j` - open table from database window (EditSource) <br />
`ctrl shift j` - open table DDL from database window (SourceEditor) <br />
`enter` - confirm change in table view (Console.TableResult.EditValue) <br />
`ctrl t` - open new console from current view (Jdbc.OpenConsole.New) <br />
`middle click` - jump to DDL - clicking on table in database window (Jdbc.OpenEditor.DDL) <br />
`ctrl f6` - modify table <br />

### macros <br />
`ctrl shift s` - reformat, rearrange, save (Macro.reformatSave) <br />
`alt t` - opening tracy folder locally in chromium (Tool_External Tools_tracy - clear exceptions) <br />
`alt shift t` - clearing exceptions in `var/tracy` (Tool_External Tools_tracy - open in chrome) <br />
`altGraph t` - run. eset to re-run tests (Run) <br />

### new files <br />
`ctrl shift comma` - new scratch. When you have selected text, opens new scratch file of appropriate file type and inserts selection (NewScratchFile) <br />
`ctrl shift period` - new php class (PhpNewClass) <br />

### opening stuff <br />
`ctrl o` - open new project/directory/file (OpenFile) <br />

### deployment <br />
`alt q` - compare with remote and send (PublishGroup.SyncLocalVsRemoteWith) <br />
`alt shift q` - sent directly to default remote (PublishGroup.Upload) <br />

## options

#### export in TSV quoted
[/options/databaseSettings.xml](/options/databaseSettings.xml)
handy when searching in DB for multiple values:  
```mysql
SELECT * 
FROM table 
WHERE id in ('f47d2411-bfbe-4d87-9e64-7879cb7dd8ba',
             'b564f37b-d829-47a0-b2e4-310d92cf7635',
             'ad671f32-81ea-4775-ad83-a817055cf6cd')
```

while TSV export is selected, you select IDS in table, press `ctrl c` and quoted ids are imploded with comma. when you're searching table connected, you `alt d` to search bar and write  
```mysql
where id in (<crtl v><backspace>)
```
you paste th eimploded ids and remove last comma. enter for showing results

#### IDE general behaviour
[/options/ide.general.xml](/options/ide.general.xml)

* no confirm on exit - if I want to exit, I do it
* new project search box starts always in USER_HOME and always opens project in new window.
* no tips on startup, thank you

## external tools
[/tools/External Tools.xml](/tools/External%20Tools.xml)

#### tracy - open in chrome
on `alt t` - opening tracy folder locally in chromium

#### tracy - clear exceptions
on `alt shift t` - clearing exceptions in `var/tracy` - in PHP written `rm $ProjectFileDir$/var/tracy/exteption*` but external tools do not support wildcards  