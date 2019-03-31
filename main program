public class main {
    public static int value;
    public static void main(String[] args) {
        value = 10;
        add target = new add();
        Sync_method sync1 = new Sync_method(target,"sync1");
        Sync_method sync2 = new Sync_method(target,"sync2");

        sync1.start();
        sync2.start();

        try {
            sync1.join();
            sync2.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        System.out.println(value);
    }
}
