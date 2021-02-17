# Java-Nimbus-Look-and-Feel-Kodlar-




import javax.swing.UIManager.*;

try {
    for (LookAndFeelInfo info : UIManager.getInstalledLookAndFeels()) {
        if ("Nimbus".equals(info.getName())) {
            UIManager.setLookAndFeel(info.getClassName());
            break;
        }
    }
} catch (Exception e) {
    // If Nimbus is not available, you can set the GUI to another look and feel.
}



// Bu şekilde run classımıza kodlarımızı yazarak veya yapıştırarak çalıştırdığımızda görüntüsü Nimbus olacaktır. 
// İmport etmeyi unutmayın.
// Kaynak: https://docs.oracle.com/javase/tutorial/uiswing/lookandfeel/nimbus.html
