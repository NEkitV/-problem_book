# -problem_book
package com.example.program;
import java.text.DateFormat;
import java.text.SimpleDateFormat;
import java.util.Date;
import java.util.Scanner;
import javafx.fxml.FXML;
import javafx.scene.control.Label;

import java.net.URL;
import java.util.ResourceBundle;
import javafx.fxml.FXML;
import javafx.scene.control.Button;
import javafx.scene.control.TextField;

public class HelloController {

    @FXML
    private ResourceBundle resources;

    @FXML
    private URL location;

    @FXML
    private Button fun;

    @FXML
    private Button save;

    @FXML
    private TextField text;

    @FXML
    void initialize() {

        System.out.println("Button Clicked!");

        Date now= new Date();

        DateFormat df = new SimpleDateFormat("dd-MM-yyyy HH:mm:ss.SSS");


        // Model Data
        String dateTimeString = df.format(now);

        // Show in VIEW
        text.setText(dateTimeString);

    }

}
