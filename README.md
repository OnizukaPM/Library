# Library
My first project.


















public class Book {
    private int id;
    private String title;
    private String authorName;
    private String authorSurname;
    private int releaseDate;
    private String category;
    private boolean isBorrowed;
    private int loans;

    public Book() {
    }

    public Book(int id, String title, String authorName, String authorSurname, int releaseDate, String category) {
        this.id = id;
        this.title = title;
        this.authorName = authorName;
        this.authorSurname = authorSurname;
        if (releaseDate <= 2017) {
            this.releaseDate = releaseDate;
        }
        this.category = category;
    }

    public int getId() {
        return id;
    }

    public String getTitle() {
        return title;
    }

    public String getAuthorName() {
        return authorName;
    }

    public String getAuthorSurname() {
        return authorSurname;
    }

    public int getReleaseDate() {
        return releaseDate;
    }

    public String getCategory() {
        return category;
    }

    public String toString() {
        return "Book " + title + " [id: " + id + ", author: "
                + authorName + " " + authorSurname + ", realease Date: "
                + releaseDate + ", category: " + category + "]";
    }
}
