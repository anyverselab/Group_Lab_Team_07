# Team Greeting Project – Group 07

This repository is for our collaborative lab project using GitHub branches and pull requests.  
Each team member will create their own `MemberX.java` file and merge it into the main branch.

---

## 🧩 GitHub Workflow Steps

### 1️⃣ Clone the main branch
Download the repository to your local machine:
```bash
git clone git@github.com:anyverselab/Group_Lab_Team_07.git
cd Group_Lab_Team_07
```

### 2️⃣ Check the current branch
Make sure you are on the **main** branch:
```bash
git branch
```

If not, switch to it:
```bash
git checkout main
```

---

### 3️⃣ Create your own feature branch
Each member creates a separate branch for their work:
```bash
git checkout -b feature-member1
```
*(Replace `member1` with your own member number.)*

---

### 4️⃣ Create and edit your Java file
Create your file under the `src/` folder. Example:
```java
public class Member1 {
    public static void main(String[] args) {
        System.out.println("Hello from Member 1!");
    }
}
```

Here is the directory structure:
```
.
├── build
│   └── classes
│       └── grouplab1
├── build.xml
├── manifest.mf
├── nbproject
│   ├── build-impl.xml
│   ├── genfiles.properties
│   ├── private
│   │   ├── private.properties
│   │   └── private.xml
│   ├── project.properties
│   └── project.xml
├── src
│   └── grouplab1
│       ├── Main.java
│       └── Member1.java (ADD MemberX.java under the grouplab1)
└── test
```

---

### 5️⃣ Add, commit, and push your changes
Save your file and run:
```bash
git add -A
git commit -m "feat: created Member1.java"
git push -u origin HEAD
```

---

### 6️⃣ Open a Pull Request (PR)
- Go to GitHub and open your branch.
- Click **“Compare & pull request.”**
- Add a short description, for example:  
  > Created `Member1.java` and uncommented `Member1.main(args)` in `Main.java`.

- Request a teammate to review your PR before merging.

---

### ✅ Notes
- Each Member should uncomment following line in their own Main.java
```
public class Main {
    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Member1.main(args);
//      Member2.main(args);  // Member 2: uncomment this line
//      Member3.main(args);  // Member 3: uncomment this line
//      Member4.main(args);  // Member 4: uncomment this line
    }
}
```


