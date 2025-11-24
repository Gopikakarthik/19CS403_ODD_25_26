# Ex.No:4(D) DESIGN PATTERN  ---- BEHAVIOUR PATTERN

## QUESTION:
Create an Article class where changes to the content are saved as mementos. Let the user view and restore any saved version.

## AIM:
To implement the Memento Design Pattern for saving, viewing, and restoring different versions of an article’s content.

## ALGORITHM :
1.	Start the program.
2. Create the Article class with methods to set content, get content, save the current state as a memento, and restore previous states.

3. Define the ArticleMemento class to store immutable snapshots of article content.

4. Maintain a list of saved versions inside the ArticleHistory class, allowing storage and retrieval of specific mementos.

5. Read multiple content updates from the user, save each as a new memento in history.

6. Read the version index to restore, retrieve the corresponding memento, restore it in the Article object, and display the restored content.
7. End the program

## PROGRAM:
 ```
/*
Program to implement a Behaviour Pattern using Java
Developed by: GOPIKA K
RegisterNumber: 212222040046 
*/
```

## SOURCE CODE:
```
import java.util.*;
class Article {
    private String content;

    public void setContent(String content) {
        this.content = content;
    }

    public String getContent() {
        return content;
    }

    public ArticleMemento save() {
        return new ArticleMemento(content);
    }

    public void restore(ArticleMemento memento) {
        this.content = memento.getContent();
    }
}

class ArticleMemento {
    private final String content;

    public ArticleMemento(String content) {
        this.content = content;
    }

    public String getContent() {
        return content;
    }
}

class ArticleHistory {
    private List<ArticleMemento> versions = new ArrayList<>();

    public void saveVersion(Article article) {
        versions.add(article.save());
    }

    public ArticleMemento getVersion(int index) {
        if (index >= 0 && index < versions.size()) {
            return versions.get(index);
        }
        return null;
    }
}

public class ArticleManager {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Article article = new Article();
        ArticleHistory history = new ArticleHistory();

        int n = Integer.parseInt(sc.nextLine());
        for (int i = 0; i < n; i++) {
            String content = sc.nextLine();
            article.setContent(content);
            history.saveVersion(article);
        }

        int restoreIndex = Integer.parseInt(sc.nextLine());
        ArticleMemento m = history.getVersion(restoreIndex);
        if (m != null) {
            article.restore(m);
            System.out.println(article.getContent());
        } else {
            System.out.println("Invalid version");
        }
    }
}
```

## OUTPUT:
<img width="887" height="523" alt="image" src="https://github.com/user-attachments/assets/b5ebeac0-c32f-4b50-9a66-97c570e08179" />


## RESULT:
The program has been executed successfully and the desired output has been obtained.

