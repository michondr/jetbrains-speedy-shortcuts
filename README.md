# PhpStorm speedy shortcuts
phpstorm settings - keymap, macros

on linux:
keymap.xml, macros.xml -> ~/.config/PhpStorm2022.3/config/options/keymapFlags.xml <br />
michondrKeymap.xml -> ~/.config/PhpStorm2022.3/keymaps <br />

## content (current window) actions
`ctrl w` - close tab (CloseContent) <br />
`ctrl shift t` - reopen closed tab (ReopenClosedTab) <br />
`ctrl shift w` - close all balast and keep current tab (CloseAllEditorsButActive) <br />

## git actions <br />
`alt w` - commit (CheckinProject) <br />
`alt e` - push (Vcs.Push) <br />
`alt r` - rebase (Git.Rebase) <br />
`altGraph a` - annotate (Annotate) <br/>
`alt shift h` - show git history of file (Vcs.ShowTabbedFileHistory) <br/>

## window actions <br />
`alt 1 (alt +)` - open/close project tree (ActivateProjectToolWindow) <br />
`alt 2 (alt ě)` - open/close database window (ActivateDatabaseToolWindow) <br />
`alt 3 (alt š)` - open/close run window (tests) (ActivateRunToolWindow) <br />
`alt 4 (alt č)` - open/close remove host (ActivateRemoteHostToolWindow) <br />
`win then e` - change from split horizontally to vertically and vice versa (ChangeSplitOrientation) <br />

## navigation <br />
`alt left (mouse back)` - Back <br />
`alt right (mouse forward)` - Forward <br />
`ctrl tab` - next tab (NextTab) <br />
`ctrl shift tab` - previous tab (PreviousTab) <br />
`ctrl alt left` - split tab to left (SplitVertically) <br />
`ctrl alt right` - split tab down (SplitHorizontally) <br />
`win then right` or `win then down` - next split screen (NextSplitter) <br />
`win then left` or `win then up` - previous split screen (PrevSplitter) <br />
`ctrl g` - go to row <br />
`ctrl e` - recent files <br />

## code tweaks <br />
`ctrl r` - refactor. works on methods, fields, classes, files. In project window can copy, move or rename files (Refactorings.QuickListPopupAction) <br />
`ctrl b (ctrl left click)` - jump to source. User to find source of method, or usages when in source <br />
`ctrl shift c` - comment whole line (CommentByLineComment) <br />
`ctrl x` - delete this line (or delete and copy selection) <br />
`alt h` - show local history (LocalHistory) <br />
`alt shift right` - move block of code 1 indent right (EditorIndentLineOrSelection) <br />
`alt shift left` - move block of code 1 indent left (EditorUnindentSelection) <br />
`alt shift up` - move block of code 1 row up <br />
`alt shift down` - move block of code 1 row down <br />
`alt up` - expand selection (EditorSelectWord) <br />
`alt down` - narrow selection (EditorUnSelectWord) <br />
`shift tab` - untab <br />
`altGraph j` - join lines <br/>
`ctrl p` - show method parameters/arguments <br />
`ctrl scrollUp` - expand region (ExpandRegion) <br />
`ctrl scrollDown` - collapse region (CollapseRegion) <br />
`ctrl shift scrollUp` - expand all regions (ExpandAllRegions) <br />
`ctrl shift scrollDown` - collapse all regions (CollapseAllRegions) <br />


## database actions <br />
`alt a` - dump to clipboard - this uses default/set dump-style (Console.TableResult.Copy.DumpToClipboard) <br />
`alt shift a` - dump to file - this uses default/set dump-style (Console.TableResult.Copy.DumpToFile) <br />
`alt c` - count rows - works in database window, or when table view (Console.TableResult.CountRows) <br />
`alt d` - filter - works like adding a where cause (Console.TableResult.EditFilterCriteria) <br />
`alt p` - transpose (Console.TableResult.Transpose) <br />
`ctrl j` - open table from database window (EditSource) <br />
`ctrl shift j` - open table DDL from database window (SourceEditor) <br />
`enter` - confirm change in table view (Console.TableResult.EditValue) <br />
`ctrl t` - open new console from current view (Jdbc.OpenConsole.New) <br />
`middle click` - jump to DDL - clicking on table in database window (Jdbc.OpenEditor.DDL) <br />
`f6` - edit table <br />

## files <br />
`ctrl shift comma` - new scratch. When you have selected text, opens new scratch file of appropriate file type and inserts selection (NewScratchFile) <br />
`ctrl shift period` - new php class (PhpNewClass) <br />
`ctrl shift i` - new php test (PhpNewTest) <br />
`alt r` - copy reference <br />
`ctrl shift alt c` - copy file absolute path (CopyContentRootPath, CopyReferencePopup, CopyReferencePopupGroup) <br />

## tests  <br />
`altGraph t` - run tests (Run) <br />
`altGraph shift t` - run failed tests (RerunFailedTests) <br />

## opening stuff <br />
`ctrl o` - open new project/directory (OpenDirectoryProject) <br />
`ctrl shift o` - open single file (OpenFile) <br />

## deployment <br />
`alt q` - compare with remote and send (PublishGroup.SyncLocalVsRemoteWith) <br />
`alt shift q` - sent directly to default remote <br />
`altGraph c` - compare with branch on git (Git.CompareWithBranch)<br />
