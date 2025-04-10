# DMS.Demo.Git.Branching.GitHubFlow.RebaseFeatureB4PR.Bad01
Steps taken to replicate:
1. Create a new class library project.
2. Add project to source control.
3. Create feature branch named 'feature/foo' & checkout.
4. Add a new class named 'Class2.cs'.
5. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #1'.
6. Commit changes: 'Branch: feature/foo | Commit #1'.
7. Checkout 'master' branch.
8. Add a comment to 'Class1.cs' : '// Branch: master | Commit #2'
9. Commit changes: 'Branch: master | Commit #2'.
10. Checkout branch 'feature/foo'.
11. Rebase branch 'feature/foo' onto 'master'.
12. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #3'
13. Commit changes: 'Branch: feature/foo | Commit #3'.
11. Add a comment to 'Class2.cs' : '// Branch: feature/foo | Commit #4'
12. Commit changes: 'Branch: feature/foo | Commit #4'.
13. Create a PR branch from 'feature/foo' named 'pull/2/merge'.
15. Push branches 'master' & 'pull/2/merge'.
16. Checkout branch 'master'.
17. Create a new pull request. Merge Into: 'master' | From: 'pull/2/merge'
18. Merge pull request.
19. Checkout branch 'master'.
20. Pull latest changes.
21. Evaluate commit history/line.

![image](https://github.com/user-attachments/assets/69197caa-0224-4fc5-9560-4b30d1b680d6)