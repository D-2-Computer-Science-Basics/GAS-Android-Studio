# GAS-Android-Studio
import android.content.Intent
import android.net.Uri
import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle

class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        // GoogleスプレッドシートのURL
        val spreadsheetUrl = "https://docs.google.com/spreadsheets/d/1qT2UVWjeVwli03yGEQf5p4KrRLWRSS9rOjd-HFGOKC8/edit?usp=sharing/edit"

        // URLを開くIntentを作成
        val intent = Intent(Intent.ACTION_VIEW, Uri.parse(spreadsheetUrl))
        startActivity(intent)
    }
}
