# PhpStorm speedy shortcuts
phpstorm settings - keymap, macros

keymap.xml, macros.xml -> C:\Users\<User>\.PhpStorm2017.2\config\options <br />
michondrKeymap.xml -> C:\Users\<User>\.PhpStorm2017.2\config\keymaps <br />

## content (current window) actions
`ctrl w` - close tab (CloseContent) <br />
`ctrl shift t` - reopen closed tab (ReopenClosedTab) <br />
`ctrl shift w` - close all balast and keep current tab (CloseAllEditorsButActive) <br />

## git actions <br />
`alt w` - commit (CheckinProject) <br />
`alt e` - push (Vcs.Push) <br />
`alt r` - rebase (Git.Rebase) <br />

## window actions <br />
`alt 1 (alt +)` - open/close project tree (ActivateProjectToolWindow) <br />
`alt 2 (alt ě)` - open/close database window (ActivateDatabaseToolWindow) <br />
`alt 3 (alt š)` - open/close database result console of current/last database tab where ran query (ActivateDatabaseConsoleToolWindow) <br />
`alt 4 (alt č)` - open/close redis (ActivateRedisServersToolWindow) <br />
`alt t` - open/close terminal window (ActivateTerminalToolWindow) <br />

## navigation <br />
`alt left (mouse back)` - Back <br />
`alt right (mouse forward)` - Forward <br />
`ctrl tab` - next tab (NextTab) <br />
`ctrl shift tab` - previous tab (PreviousTab) <br />
`ctrl alt left` - split tab to left (SplitVertically) <br />
`ctrl alt right` - split tab down (SplitHorizontally) <br />
`alt m` - next split screen (NextSplitter) <br />
`alt n` - previous split screen (PrevSplitter) <br />

## code tweaks <br />
`ctrl r` - refactor. works on methods, fields, classes, files. In project window can copy, move or rename files (Refactorings.QuickListPopupAction) <br />
`ctrl b (ctrl left click)` - jump to source. User to find source of method, or usages when in source <br />
`ctrl shift c` - comment whole line (CommentByLineComment) <br />
`ctrl x` - delete this line (or delete and copy selection) <br />
`alt h` - show local history (LocalHistory) <br />
`alt shift right` - move block of code 1 indent right (EditorIndentLineOrSelection) <br />
`alt shift left` - move block of code 1 indent left (EditorUnindentSelection) <br />
`alt up` - expand selection (EditorSelectWord) <br />
`alt down` - narrow selection (EditorUnSelectWord) <br />
`shift tab` - untab <br />

## database actions <br />
`alt a` - dump to clipboard - this uses default/set dump-style (Console.TableResult.Copy.DumpToClipboard) <br />
`alt shift a` - dump to file - this uses default/set dump-style (Console.TableResult.Copy.DumpToFile) <br />
`alt c` - count rows - works in database window, or when table view (Console.TableResult.CountRows) <br />
`alt d` - filter - works like adding a where cause (Console.TableResult.EditFilterCriteria) <br />
`alt p` - transpose (Console.TableResult.Transpose) <br />
`ctrl j` - open table from database window (EditSource) <br />
`enter` - confirm change in table view (Console.TableResult.EditValue) <br />
`ctrl t` - open new console from current view (Jdbc.OpenConsole.New) <br />
`middle click` - jump to DDL - clicking on table in database window (Jdbc.OpenEditor.DDL) <br />
`f6` - edit table <br />

## macros <br />
`ctrl shift s` - reformat, rearrange, save (Macro.reformatSave) <br />
`alt s` - add current class to services (Tool_External Tools_AddService BIN/CONSOLE) <br />
`alt semicolon` - close all (Macro.clear workspace) - works only on windows <br />
`altGraph t` - surround current selection for translate (Macro.pushTranslate) - works in twig <br />

## new files <br />
`ctrl shift comma` - new scratch. When you have selected text, opens new scratch file of appropriate file type and inserts selection (NewScratchFile) <br />
`ctrl shift period` - new php class (PhpNewClass) <br />

## opening stuff <br />
`ctrl o` - open new project/directory (OpenDirectoryProject) <br />
`ctrl shift o` - open single file (OpenFile) <br />

## deployment <br />
`alt q` - compare with remote and send (PublishGroup.SyncLocalVsRemoteWith) <br />
`alt shift q` - sent directly to default remote <br />
