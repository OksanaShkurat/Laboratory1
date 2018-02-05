# Laboratory1
import javafx.scene.paint.Color;
import javafx.application.Application;
import javafx.scene.Group;
import javafx.scene.Scene;
import javafx.stage.Stage;
import javafx.scene.shape.*;
import javafx.scene.paint.Color;

public class MyJavaFXApplication extends Application {
    public static void main(String[] args) {
        launch(args);
    }

    @Override
    public void start(Stage primaryStage) {        
        Group root = new Group();
        Scene scene = new Scene(root, 300, 250);
//////////////////////////////////////////////////////
//елементи сцени будемо вставляти сюди

        Rectangle r = new Rectangle(50, 50, 200, 100); //створення фігури
        root.getChildren().add(r); //додавання фігури до кореневого контейнера
        r.setFill(Color.YELLOW);; //Встановимо жовтий колір за допомогою константи
        scene.setFill(Color.GREEN); //Встановимо зелений фон за допомогою константи

        Line l = new Line(100, 100, 200, 100); //
        root.getChildren().add(l);
        l.setStroke(Color.RED);

//////////////////////////////////////////////////////
        primaryStage.setScene(scene);
        primaryStage.show();
    }
}
