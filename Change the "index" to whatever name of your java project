import javax.swing.*;
import java.awt.*;

public class index {
    public static void main(String[] args) {
        SwingUtilities.invokeLater(() -> {
            JFrame frame = new JFrame("Java Logo by Kishan Yadav");
            frame.setSize(1600, 900);
            frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

            JPanel panel = new JPanel() {
                @Override
                protected void paintComponent(Graphics g) {
                    super.paintComponent(g);
                    drawRainbow(g);
                    drawJavaLogo(g);
                }
            };

            frame.add(panel);
            frame.setVisible(true);
        });
    }

    private static void drawJavaLogo(Graphics g) {
        g.setColor(Color.GREEN);
        g.fillOval(50, 50, 200, 200);

        g.setColor(Color.YELLOW);
        g.fillArc(60, 60, 180, 180, 0, 180);

        g.setColor(Color.BLACK);
        g.setFont(new Font("Arial", Font.BOLD, 40));
        g.drawString("!JAVA!", 95, 160);
    }

    private static void drawRainbow(Graphics g) {
        int x = 0;
        int y = 0;
        int width = 300;
        int height = 300;
        int[] rainbowColors = {255, 127, 0, 255, 255, 0, 0, 255, 0};

        for (int i = 0; i < 9; i++) {
            g.setColor(new Color(rainbowColors[i], 0, 255 - rainbowColors[i]));
            g.fillArc(x, y, width, height, 0, 360);
            width -= 10;
            height -= 10;
            x += 5;
            y += 5;
        }
    }
}
