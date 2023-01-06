# PhpStorm speedy shortcuts
phpstorm settings - keymap, macros

on linux:
keymap.xml -> ~/.config/PhpStorm2022.3/config/options/keymapFlags.xml  
macros.xml -> ~/.config/PhpStorm2022.3/config/options/macros.xml  
michondrKeymap.xml -> ~/.config/PhpStorm2022.3/keymaps  

you can symlink these (don't forget to edit location where you've cloned the repo)

```shell
ln -s ~/_michondr/speedy-shortcuts/michondrKeymap.xml ~/.config/JetBrains/PhpStorm2022.3/keymaps/michondrKeymap.xml
ln -s ~/_michondr/speedy-shortcuts/keymap.xml ~/.config/JetBrains/PhpStorm2022.3/options/keymapFlags.xml
ln -s ~/_michondr/speedy-shortcuts/macros.xml ~/.config/JetBrains/PhpStorm2022.3/options/macros.xml
```

## content (tab window) actions
`ctrl w` - close tab (CloseContent)  
`ctrl shift t` - reopen closed tab (ReopenClosedTab)  
`ctrl shift w` - close all balast and keep current tab (CloseAllEditorsButActive)  
`ctrl tab` - next tab (NextTab)  
`ctrl shift tab` - previous tab (PreviousTab)  
`ctrl alt left` - split tab to left (SplitVertically)  
`ctrl alt right` - split tab down (SplitHorizontally)  
`win then right` or `win then down` - next split screen (NextSplitter)  
`win then left` or `win then up` - previous split screen (PrevSplitter)  
`win then e` - change from split horizontally to vertically and vice versa (ChangeSplitOrientation)

## git actions
`alt w` - commit (CheckinProject)  
`alt e` - push (Vcs.Push)  
`alt r` - rebase (Git.Rebase)  
`altGraph a` - annotate (Annotate) <br/>
`alt shift h` - show git history of file (Vcs.ShowTabbedFileHistory) <br/>

## window actions
`alt 1 (alt +)` - open/close project tree (ActivateProjectToolWindow)  
`alt 2 (alt ě)` - open/close database window (ActivateDatabaseToolWindow)  
`alt 3 (alt š)` - open/close run window (tests) (ActivateRunToolWindow)  
`alt 4 (alt č)` - open/close remove host (ActivateRemoteHostToolWindow)  

## navigation
`alt left (mouse back)` - Back  
`alt right (mouse forward)` - Forward  
`ctrl g` - go to row  
`ctrl e` - recent files  

## code tweaks
`ctrl r` - refactor. works on methods, fields, classes, files. In project window can copy, move or rename files (Refactorings.QuickListPopupAction)  
`ctrl b (ctrl left click)` - jump to source. User to find source of method, or usages when in source  
`ctrl shift c` - comment whole line (CommentByLineComment)  
`ctrl x` - delete this line (or delete and copy selection)  
`alt h` - show local history (LocalHistory)  
`alt shift right` - move block of code 1 indent right (EditorIndentLineOrSelection)  
`alt shift left` - move block of code 1 indent left (EditorUnindentSelection)  
`alt shift up` - move block of code 1 row up  
`alt shift down` - move block of code 1 row down  
`alt up` - expand selection (EditorSelectWord)  
`alt down` - narrow selection (EditorUnSelectWord)  
`shift tab` - untab  
`altGraph j` - join lines <br/>
`ctrl p` - show method parameters/arguments  
`ctrl scrollDown` - expand region (ExpandRegion)  
`ctrl scrollUp` - collapse region (CollapseRegion)  
`ctrl shift scrollDown` - expand all regions (ExpandAllRegions)  
`ctrl shift scrollUp` - collapse all regions (CollapseAllRegions)  


## database actions
`alt a` - dump to clipboard - this uses default/set dump-style (Console.TableResult.Copy.DumpToClipboard)  
`alt shift a` - dump to file - this uses default/set dump-style (Console.TableResult.Copy.DumpToFile)  
`alt c` - count rows - works in database window, or when table view (Console.TableResult.CountRows)  
`alt d` - filter - works like adding a where cause (Console.TableResult.EditFilterCriteria)  
`alt p` - transpose (Console.TableResult.Transpose)  
`ctrl j` - open table from database window (EditSource)  
`ctrl shift j` - open table DDL from database window (SourceEditor)  
`enter` - confirm change in table view (Console.TableResult.EditValue)  
`ctrl t` - open new console from current view (Jdbc.OpenConsole.New)  
`middle click` - jump to DDL - clicking on table in database window (Jdbc.OpenEditor.DDL)  
`f6` - edit table  

## files
`ctrl shift comma` - new scratch. When you have selected text, opens new scratch file of appropriate file type and inserts selection (NewScratchFile)  
`ctrl shift period` - new php class (PhpNewClass)  
`ctrl shift i` - new php test (PhpNewTest)  
`alt r` - copy reference  
`ctrl shift alt c` - copy file absolute path (CopyContentRootPath, CopyReferencePopup, CopyReferencePopupGroup)  

## tests
`altGraph t` - run tests (Run)  
`altGraph shift t` - run failed tests (RerunFailedTests)  

## macros
`ctrl shift s` - refactor core, rearrange, save (RearrangeCode, ReformatCode, SaveAll)

## opening stuff
`ctrl o` - open new project/directory (OpenDirectoryProject)  
`ctrl shift o` - open single file (OpenFile)  

## deployment
`alt q` - compare with remote and send (PublishGroup.SyncLocalVsRemoteWith)  
`alt shift q` - sent directly to default remote  
`altGraph c` - compare with branch on git (Git.CompareWithBranch)<br />
