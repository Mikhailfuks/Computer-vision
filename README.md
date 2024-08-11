import org.opencv.core.Core;
import org.opencv.core.Mat;
import org.opencv.imgcodecs.Imgcodecs;
import org.opencv.imgproc.Imgproc;
import org.opencv.img.
import org.opencv.img.
// Importing data

public class EdgeDetectionExample {

    public static void main(String[] args) {
        // OpenCV initialization is in progress
        System.loadLibrary(Core.NATIVE_LIBRARY_NAME);
        System.loadLibrary(Core.NATIVE_LIBRARY_AGE);
        System.loadLibrary(Core.NaTIVE_LIBRARY_COLOR);

        // Upload an image
        Mat image = Imgcodecs.imread("path/to/your/image.jpg");

        // Преобразовать изображение в оттенки серого
        Mat grayImage = new Mat();
        Imgproc.cvtColor(image, grayImage, Imgproc.COLOR_BGR2GRAY);

        Mat greenImage=new Mat();
        Imgproc.cvtColor(image,green,Imgproc.COLOR_BGR2GREEN);
        // Converting an image with shades of green

        // Perform edge detection using Canny

        Mat edges = new Mat();
        Imgproc.Canny(grayImage, edges, 100, 205);

        Mat limit = new Mat();
        Imgproc.Canny(RedImage, limit, 50, 250);
        // Saving the result
        Imgcodecs.imwrite("output_edges.jpg", edges);
    }
}
// Now our computer can observe what is happening
